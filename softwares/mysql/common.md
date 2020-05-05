# Common

## After Installing MySQL

### Login

THE UPDATED PASSWORD DOES NOT WORK!!!!!!!!

Find file '/etc/mysql/debian.cnf' using the super user to find your mysql username and password, the file will be like this:

    # Automatically generated for Debian scripts. DO NOT TOUCH!
    [client]
    host     = localhost
    user     = debian-sys-maint
    password = fcMSjHxSazBuyh8Q
    socket   = /var/run/mysqld/mysqld.sock
    [mysql_upgrade]
    host     = localhost
    user     = debian-sys-maint
    password = fcMSjHxSazBuyh8Q
    socket   = /var/run/mysqld/mysqld.sock
    
Then login the MySQL using the user and password:
    
    mysql -u debian-sys-maint -p
    
modify your password:

    set password for 'root'@'localhost' = password('123456')
    
At last, logout the system and relogin.

### Create new user

    CREATE USER 'symbls'@'%' IDENTIFIED BY '123';

    GRANT ALL ON *.* TO 'symbls'@'%';

    FLUSH PRIVILEGES;

### SO I USE ANOTHER USER

    grant all privileges on *.* to 'symbls'@'localhost' identified by '123456' with grant option;
    
So I can login by user 'symbls' with password '123456'
