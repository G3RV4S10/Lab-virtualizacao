Incluir:
Passo a passo da instalação do ESXi.
Como configurar e adicionar hosts no vSphere.

# Instruções de instalação do VMware ESXi 6

## Instalando o ESXi em um pendrive
Depois de colocar o cartão SD no seu sistema, encontre o instalador do ESXi que você criou seguindo os passos de download do instalador.

Para instalar o ESXi no pendrive ou cartão SD, siga estes passos:

Ligue o sistema.
IMPORTANTE: Antes de instalar o ESXi, ative o dispositivo de armazenamento (pendrive ou cartão SD). Para mais detalhes, veja como ativar ou desativar o armazenamento flash.

Insira o pendrive ou disco com o instalador do ESXi no computador.

Reinicie o sistema.

Quando o logo da Dell aparecer, pressione F11 imediatamente para acessar o menu de boot.

No menu de boot, use as setas do teclado para selecionar o dispositivo onde está o instalador do ESXi (como um pendrive ou unidade de DVD) e pressione Enter. O processo de instalação será iniciado.

ATENÇÃO: O próximo passo apagará todos os dados do pendrive ou cartão SD escolhido para a instalação.

Na tela de seleção de disco, escolha o pendrive ou cartão SD onde deseja instalar o ESXi e pressione Enter.

Defina uma senha para o usuário root e pressione F11 para iniciar a instalação.

Quando a instalação terminar, pressione Enter para reiniciar o sistema.

Quando o logo da Dell aparecer novamente, pressione F11 imediatamente.

No menu de boot, use as setas do teclado para selecionar o pendrive ou cartão SD onde o ESXi foi instalado e pressione Enter. O sistema vai iniciar o ESXi.

Para que o ESXi inicie automaticamente sempre que ligar o computador, configure a sequência de boot no BIOS.

Por fim, ative a licença correta do ESXi. Para mais informações, consulte a seção sobre licenciamento.

