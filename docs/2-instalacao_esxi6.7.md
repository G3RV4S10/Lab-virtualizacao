Incluir:
Passo a passo da instalação do ESXi.
Como configurar e adicionar hosts no vSphere.

Instalando o ESXi em mídia flash
Depois de instalar o cartão SD no seu sistema, localize a mídia do instalador do ESXi que você criou em Baixando a mídia do instalador do ESXi .
Para instalar o ESXi na mídia flash, conclua as seguintes etapas:
Ligue o sistema.
NOTA: Antes de instalar o ESXi, habilite o dispositivo de armazenamento flash. Para obter mais informações, consulte Habilitando ou desabilitando o dispositivo de armazenamento flash .
Insira a mídia do instalador do ESXi na unidade óptica.
Reinicie o sistema.
Quando o logotipo da Dell for exibido, pressione F11 imediatamente.
No Boot Menu , use as teclas de seta para cima e para baixo para selecionar a unidade óptica e pressione Enter. O ambiente do instalador inicia. Quando a imagem do instalador carrega, o sistema está pronto para começar o processo de criação de imagens de armazenamento flash.
CUIDADO: A etapa 6 exclui todos os dados do dispositivo de armazenamento SD.
Na página Selecionar um disco , selecione o dispositivo de armazenamento SD no qual você deseja instalar o ESXi e pressione Enter.
Digite a senha de root e pressione F11 para iniciar a instalação.
Quando o processo de instalação estiver concluído, pressione Enter para reiniciar o sistema.
Quando o logotipo da Dell for exibido, pressione F11 imediatamente.
No Boot Menu , use as teclas de seta para cima e para baixo para selecionar o dispositivo de armazenamento SD e pressione Enter. O sistema inicializa e inicia o ESXi.
Para habilitar a inicialização recorrente, consulte Configurando a sequência de inicialização para ESXi .
Defina o modo de licenciamento correto. Para obter mais informações, consulte Informações sobre licenciamento .
