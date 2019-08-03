# MariaDB

MariaDB é um banco de dados que surgiu como derivação do MySQL, criado pelo próprio fundador do projeto após sua aquisição pela Oracle.

## Instalação

Toda a instalação é feita como **root**

### Debian

Instale o pacote mariadb-server com o comando:

 `apt-get install mariadb-server`

### CentOs

Instale o pacote mariadb-server com o comando:

 `yum -y install mariadb-server`

## Configuração

### CentOs

Chame o configurador do MariaDB-server com o comando:

 `mysql_secure_installation`

## Phpmyadmin

Dependências:

Apache / Httpd ou Nginx instalado e configurado.  
PHP instalado

### Debian

Instale o wget com o comando:

 `apt-get install wget`

Instale o php-mbstring com o comando:

 `apt-get install php-mbstring`  
  
Instale o php-mysql com o comando:

`apt-get install php-mysql`

### CentOs

 Istale o wget com o comando:

 `yum -y install wget`

Instale o php-mbstring com o comando:

 `yum -y install php-mbstring`

Instale o php-mysql com o comando:

 `yum -y install php-mysql`

### Comum a ambos

Baixe o phpmyadmin com o comando:

 `wget https://files.phpmyadmin.net/snapshots/phpMyAdmin-4.9+snapshot-all-languages.tar.gz`

Extraia o conteúdo do phpMyAdmin-4.9+snapshot-all-languages.tar.gz com o comando:

 `tar -xvzf phpMyAdmin-4.9+snapshot-all-languages.tar.gz`

Mova a pasta phpMyAdmin-4.9+snapshot-all-languages para a pasta /var/www/html com o comando:

 `mv phpMyAdmin-4.9+snapshot-all-languages /var/www/html/phpMyAdmin
`

### Após a instalação

### Debian

Reinicie o serviço do Apache com o comando:

 `service apache2 restart`

### CentOs

Reinicie o serviço do Httpd com o comando:

 `service httpd restart`

## Testes

 `Teste abra o ip do servidor /phpmyadmin no navegador`