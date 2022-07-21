# Acessar maquina via ssh sem senha
## 1. Na máquina de origem (maquina 1), execute o comando
- $ ssh-keygen -t rsa -f ~/.ssh/id_rsa

Esse comando é usasdo para produzir uma chave de autenticação ssh.

Após executado, começara a aparecer um monte de comandos na tela, aperte enter até sua chave ser criada.

A chave sera guardada no diretório /home/usuario/.ssh/

No lugar de usuario será o nome do usuário que executou o comando.

Agora é preciso mandar essa chave para a máquina que você deseja conectar (maquina 2).

## 2. Na maquina de origem (maquina 1) execute o comando 
- ssh-copy-id ip-da-maquina

No lugar de ip-da-maquina você deve colocar o ip da máquina que você deseja conectar (maquina 2). Esse comando copia a chave da maquina de origem (maquina 1) para a outra maquina (maquina 2).

*Esse processo permite apenas que você se conecte na maquina 1 a maquina 2 sem senha. Para se conectar da maquina 2 para a maquina 1 sem senha é preciso repetir o processo na maquina 2*
