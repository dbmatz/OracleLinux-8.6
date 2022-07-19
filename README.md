# OracleLinux-8.6

- Baixar full ISO Oracle 8.6

## 1. Selecionar idioma
É recomendado selecionar o inglês por ser o primeiro a receber novas versões.
## 2. Localization
### 2.1 Selecionar idioma do teclado (Keyboard)
Caso você tenha selecionado inglês na primeira parte o linux automáticamente deixa seu teclado como padrão inglês. Para trocar é so tirar o English e adicionar o Portuguese (Brazil)
### 2.2 Configurar data e hora (Time & Date)
Nesta parte é onde é configurado a data e hora que o sistema deve receber.
## 3. Software
### 3.1 Escolher software (Software selection)
O Oracle linux tem várias opções de software. Vou usar o minimal install por ser mais leve e possuir apenas o necessário.
## 4. System
### 4.1 Fazer repartições (Installation Destination)
Nesta parte é feita a repartição do disco virtual. Como meu disco é de 20GB a repartição fica assim
5GiB para o filesystem /var/lib/docker (nesse filesystem será usado o formato ext4)
3GiB para o filesystem /
3GiB para o filesystem /var
3GiB para o filesystem /tmp
3GiB para o filesystem /home
### 4.2 Internet e nome da máquina (Network e Host Name)
Para ter acesso a internet troca o off para on. Para trocar o nome da máquina é só alterar a parte onde diz 'Host Name:' para o nome desejado para exemplo.localdomain
## 5.User settings
### 5.1 Senha do Root (Root Password)
Aqui é definido a senha do usuário Root.
### 5.2 Criar usuário (User Creation)
Nesa parte é criado o primeiro usuário da máquina, aqui já é possivel definir o usuário como adminitrador (Sudoer).
