# Instalando o ESXi em um Pendrive

## Passos para a instalação  

1. **Ligue o sistema.**  

2. **Insira o pendrive ou disco com o instalador do ESXi no Servidor.**  

3. **Quando o logo da Dell aparecer, pressione `F11` imediatamente para acessar o menu de boot.**  
OBS: Metodo utilizado no Poweredge r910. Talvez sua maquina o metodo seja outro

4. **No menu de boot, use as setas do teclado para selecionar o dispositivo onde está o instalador do ESXi**  
   (como um pendrive ou unidade de DVD) e pressione `Enter`. O processo de instalação será iniciado.

![image](https://github.com/user-attachments/assets/e861ffee-3bc8-4bc7-aad0-6b5a9974ba8a)
Espere carregar todos os módulos.

6. **Na tela de boas vindas tecle `ENTER` para continuar.**  
![image](https://github.com/user-attachments/assets/c700e8d8-27e6-437d-8301-13516fd5a92c)


7. **Pressione F11 para aceitar o termo.**  
![image](https://github.com/user-attachments/assets/1e6e97d0-9ef2-4255-a07d-bd6fd2d30303)

8. **Selecione o hd onde será instalado o seu hypervisor.**  
![image](https://github.com/user-attachments/assets/af0b356f-b54a-4f42-8f75-e7ec3f1d3f3b)
OBS: Caso encontre algum problema e/ou hd não apareça, verifique o drive da controladora se é compativel com a versão. E/ou atualize os drives

9. **Insira a senha de acordo com sua preferencia e lembre de assegurar uma senha que contenha letras+números+caracter especial, afinal, é a entrada de sua infra.**  
![image](https://github.com/user-attachments/assets/2a216dc1-3de6-4dea-a861-129ffb8025aa)

10. **Confirme os dados inseridos ate esse ponto e inicie a instalação usando a tecla F11.**  
![image](https://github.com/user-attachments/assets/267749ea-812f-4644-b3bf-f53a39e97ffe)

11. **Aguarde o processamento(Instalação do Esxi).**
![image](https://github.com/user-attachments/assets/2a84cfb1-1b1d-4e9c-a791-dacd1fcdcda2)


12. **Após a reinicialização, a tela de login estará disponível para ser customizado de acordo com sua necessidade, neste caso o DHCP entregou o ip ao servidor, mas pressionando a tecla F2 poderá ser alterado/adicionado o IP de sua preferencia para o servidor.**  
![image](https://github.com/user-attachments/assets/9df37f18-36af-456d-82d4-dd4790b35e38)
OBS: Como supracitado, altere de acordo com sua necessidade, este ip será o acesso ao gerenciador WEB da interface do hypervisor

13. **Alteração do IP**
![image](https://github.com/user-attachments/assets/3793212b-4184-4173-80f3-af9da4d57fdb)
OBS: Ao pressionar `F2` será solicitado a senha root

14. **Após a customização do endereço, acesse o navegador e aponte o IP que foi informado para acesso ao gerenciador WEB da interface do hypervisor.**
![image](https://github.com/user-attachments/assets/c4c98b87-ebd6-4ba6-9610-9802643e9822)

15. **Pronto, seu hypervisor VMWare ESXI 6.5 esta instalado e pronto para ser usado em sua infra**
![image](https://github.com/user-attachments/assets/81ecd089-098b-4784-a4b4-3399e443d739)

16. **Por fim, ative a licença correta do ESXi.**

**Imagem do nosso hypervisor esxi 6.7 instalado e sendo utilizado.**
![image](https://github.com/user-attachments/assets/81b28685-384a-4dee-bdd2-24e806d0e66e)

