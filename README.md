# OracleLinux-8.6

- Baixar full ISO Oracle *versão 8.6*- https://yum.oracle.com/oracle-linux-isos.html
- Fazer a instalação da Oracle VM Virtual Box *versão 6.1* - https://www.virtualbox.org/

## Configurações da VM
### 1. Na parte superior da VM selecione Novo.
### 2. Criação da Maquina Virtual.
Após, ira abrir a janela de criação, nela pode ser configurado o nome, pasta onde a maquina sera guardada, tipo de sistema operacional que sera usuado na maquina e versão do sistema operacional.
- Nome: Oracle Linux 8.6
- Tipo: Linux
- Versão: Oracle (64-bit)
### 3. Repartição da memória RAM
Está parte diz respeito a quantidade de memória RAM que será dedicado a máquina virtual.
- 1560 mb
### 4. Criar disco rígido virtual
Este disco sera usado pela máquina. Como não possui um, tem que criar.
- Criar disco rígido virtual agora
#### 4.1 Tipos de arquivo de disco rígido
Escolher o tipo do disco. Vai criar um disco virtual.
- VDI (Virtual Disk Image)
#### 4.2 Armazenamento em disco rígido físico
Escolha o tipo do disco virtual.
- Tamanho fixo
#### 4.3 Localização e tamanho do arquivo
Informe o nome do arquivo onde ficara o disco virtual e o tamanho, esse tamanho é o limite máximo de dados que uma máquina virtual poderá armazenar neste disco rígido.
- 20,00 GB
### 5. Selecione o disco rígido de boot
Selecione a ISO do sistema operacional. Aperte na pasta amarela.
#### 5.1 Seletor de discos ópticos
Vá em acrescentar e seleciona a ISO Oracle Linux 8.6.

## Instalação ISO 
### 1. Selecionar idioma
É recomendado selecionar o inglês por ser o primeiro a receber novas versões.
### 2. Localization
#### 2.1 Selecionar idioma do teclado (Keyboard)
Caso você tenha selecionado inglês na primeira parte o linux automáticamente deixa seu teclado como padrão inglês. Para trocar é so tirar o English e adicionar o Portuguese (Brazil)
#### 2.2 Configurar data e hora (Time & Date)
Nesta parte é onde é configurado a data e hora que o sistema deve receber.
### 3. Software
#### 3.1 Escolher software (Software selection)
O Oracle linux tem várias opções de software. Vou usar o minimal install por ser mais leve e possuir apenas o necessário.
### 4. System
#### 4.1 Fazer repartições (Installation Destination)
Nesta parte é feita a repartição do disco virtual. Como meu disco é de 20GB a repartição fica assim
5GiB para o filesystem /var/lib/docker (nesse filesystem será usado o formato ext4)
3GiB para o filesystem /
3GiB para o filesystem /var
3GiB para o filesystem /tmp
3GiB para o filesystem /home
#### 4.2 Internet e nome da máquina (Network e Host Name)
Para ter acesso a internet troca o off para on. Para trocar o nome da máquina é só alterar a parte onde diz 'Host Name:' para o nome desejado para exemplo.localdomain
### 5.User settings
#### 5.1 Senha do Root (Root Password)
Aqui é definido a senha do usuário Root.
#### 5.2 Criar usuário (User Creation)
Nessa parte é criado o primeiro usuário da máquina, aqui já é possivel definir o usuário como adminitrador (Sudoer).
