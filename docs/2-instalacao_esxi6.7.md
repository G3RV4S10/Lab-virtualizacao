# Instalando o ESXi em um Pendrive

## Passos para a instalação  

1. **Ligue o sistema.**  
   > **IMPORTANTE:** Antes de instalar o ESXi, ative o dispositivo de armazenamento (pendrive ou cartão SD). Para mais detalhes, veja como ativar ou desativar o armazenamento flash.  

2. **Insira o pendrive ou disco com o instalador do ESXi no computador.**  

3. **Reinicie o sistema.**  

4. **Quando o logo da Dell aparecer, pressione `F11` imediatamente para acessar o menu de boot.**  
OBS: Metodo utilizado no Poweredge r910. Talvez sua maquina o metodo seja outro

5. **No menu de boot, use as setas do teclado para selecionar o dispositivo onde está o instalador do ESXi**  
   (como um pendrive ou unidade de DVD) e pressione `Enter`. O processo de instalação será iniciado.
   ![image](https://github.com/user-attachments/assets/b8584b42-f90c-4862-bbb2-26ba913ed3a0)
 
7. ⚠ **ATENÇÃO:** O próximo passo apagará todos os dados do pendrive ou cartão SD escolhido para a instalação.  

8. **Na tela de seleção de disco, escolha o pendrive ou cartão SD onde deseja instalar o ESXi e pressione `Enter`.**  

9. **Defina uma senha para o usuário `root` e pressione `F11` para iniciar a instalação.**  

10. **Quando a instalação terminar, pressione `Enter` para reiniciar o sistema.**  

11. **Quando o logo da Dell aparecer novamente, pressione `F11` imediatamente.**  

12. **No menu de boot, use as setas do teclado para selecionar o pendrive ou cartão SD onde o ESXi foi instalado e pressione `Enter`.**  
    O sistema vai iniciar o ESXi.  

13. **Para que o ESXi inicie automaticamente sempre que ligar o computador, configure a sequência de boot no BIOS.**  

14. **Por fim, ative a licença correta do ESXi.**
