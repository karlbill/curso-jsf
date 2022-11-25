# Curso JSF
Estudo sobre o framework Java Server Faces (JSF)

## Instalação das ferramentas (Ubuntu - WSL2)
1. Instalação do Java usando o sdkman!: ``` sdk list java ``` ``` sdk install java 8.0.352-albba ``` ``` java --version```
2. Instalação do MySQL: ``` sudo apt update ``` ``` sudo apt install mysql-server ``` ``` mysql --version ```

Links: 
1. [SDK! site](https://sdkman.io/usage)
2. [MySQL Instalation](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-database)

## Iniciando o MySQL
1. Instanciando o MySQL: ``` sudo /etc/init.d/mysql start ```
2. Configurando uma senha para o usuário root: ``` sudo mysql_secure_installation ```
> Caso seja necessário reiniciar a senha do root, os seguintes passos devem ser seguidos
> 1. Alterar o arquivo my.cnf: ``` sudo nano /etc/mysql/my.cnf ``` , incluindo as linhas ``` [mysqld] ``` e ``` skip-grant-tables ```
> 2. Reiniciar o serviço do MySQL: ``` sudo /etc/init.d/mysql restart ```
> 3. Acessar o MySQL pelo seguinte comando: ``` sudo mysql -u root -p ``` (Acessar sem senha)
> 4. Dentro do MySQL, usar o comando ``` flush privileges; ``` para que seja possível alterar a senha do root com o servidor em execução
> 5. Alterar a senha do root: ``` ALTER USER 'root'@'localhost' IDENTIFIED BY 'MyNewPass'; ```
> 6. Sair do MySQL e remover a linha ``` skip-grant-tables ``` do arquivo **my.cnf** anteriormente modificado.
> 7. Reiniciar o servidor: ``` sudo /etc/init.d/mysql restart ```





















