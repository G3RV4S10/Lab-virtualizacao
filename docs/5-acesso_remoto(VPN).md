Incluir:
Como configurar a VPN PPTP.  
Criar contas para acesso.  


VM ubuntu utilizada dentro do nosso ambiente vsphere
Instalando o servidor pptp na vm ubuntu
sudo apt install pptpd

nano /etc/ppp/pptpd-options
Neste exemplo deixarei um print do arquivo, configuração a configuração padrão e esta:
ms-dns 8.8.8.8 - Ou um de sua preferencia
ms-dns 8.8.4.4 Ou um DNS alternativo de sua preferencia
name pptpd
refuse-pap
refuse-chap
refuse-mschap
require-mschap-v2
require-mppe-128
require-mppe-40
noccp

edite-o
nano /etc/pptpd.conf
Altere de acordo com sua rede
localip 10.0.0.1
remoteip 10.0.0.100-200
Onde localip é o endereço IP do seu servidor e remoteip é o range de IPs que serão atribuídos aos clientes que se conectarem a ele.

#IP do Servidor da VPN
localip 172.31.255.1
#Range de IPs que serão atribuídos aos dispositivos conectados na VPN
remoteip 172.31.255.2-30

Em seguida, você deve configurar a autenticação para PPTP adicionando usuários e senhas. 
Configurando a autenticação para PPTP, Adicionando usuários e senhas
Basta adicioná-los a /etc/ppp/chap-secrets:
sudo nano /etc/ppp/chap

Configurando forwading(encaminhamento) É importante habilitar o encaminhamento de IP no seu servidor PPTP. Isso permitirá que você encaminhe pacotes entre IPs públicos e privados configurados com PPTP. Basta editar /etc/sysctl.conf e adicionar a seguinte linha, caso ela ainda não exista:
nano /etc/sysctl.conf
# Uncomment the next line to enable packet forwarding for IPv4
Ou adicione-a no final do arquivo caso não tenha 
net.ipv4.ip_forward=1


Create a NAT rule for iptables
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE && iptables-save
That's it. You've successfully Created your own PPTP VPN Server
Now You can Login and Use your Personal

iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE && iptables-save

Etapa 4 - Crie uma regra NAT para iptables
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE && iptables-save


Se você também quiser que seus clientes PPTP se comuniquem entre si, adicione as seguintes regras do iptables:
iptables --table nat --append POSTROUTING --out-interface ppp0 -j MASQUERADE
iptables -I INPUT -s 10.0.0.0/8 -i ppp0 -j ACCEPT
iptables --append FORWARD --in-interface eth0 -j ACCEPT

