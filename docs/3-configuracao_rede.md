## Pré-requisitos

Para este ambiente, foi utilizada uma instalação do ESXi em um servidor físico, podendo ser replicado também em desktops compatíveis.

---

# Configuração Inicial de Rede no ESXi

A configuração de rede foi realizada diretamente pelo console do ESXi, acessado com a conta de administrador `root`.  

No menu principal, foi selecionada a opção `Configure Management Network`, onde foram definidos os parâmetros de rede conforme a topologia do laboratório.

![Tela de configuração de rede do ESXi](https://github.com/user-attachments/assets/3241e216-9684-4f31-930e-1c86a6404171)

A rede foi configurada com base na estrutura existente do ambiente, respeitando as VLANs previamente definidas no switch gerenciável. Quando necessário, o ID da VLAN foi especificado para garantir a comunicação adequada com os demais recursos do laboratório.

---

*Observação:* todas as definições de rede foram ajustadas para garantir conectividade com os hosts do vSphere.
