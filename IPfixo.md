# Configurar IP fixo no modo bridge
 Para configurar o IP fixo no modo bridge será usado o networkmanager TUI, que pode ser acessado através do comando nmtui.
## 1. $ nmtui
## 2. Selecionar a opção Edit a connection
## 3. Selecione a conexão que deseja configurar o ip fixo e depois vá em <Edit...>. 
Será então aberto a tela de edição da rede. Se o endereço ip estiver sendo denominado pelo dhcp a configuração aparecerá como <Automatic>.
## 4. Troque de Automatic para Manual, em seguida vá em show. 
 O addresses é referente ao endereço ip, como ainda não foi configurado não aparece nada.
## 5. Após inserido o IP e o gateway desejado é só salvar e reiniciar a internet (systemctl restart network) ou reiniciar a máquina (reboot).
