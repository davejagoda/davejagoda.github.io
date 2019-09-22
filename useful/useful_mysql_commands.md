---
title: Useful MySQL commands
layout: appleII
---

from command line
-----------------

`mysqld --datadir ~/db/mysql5.7`

`mysqladmin -u root -p shutdown`

`mysql -u <username> -p <dbname>`

`mysql -u <username> -p<password> <dbname>`

`mysqladmin -u <username> -p create <dbname>`

`mysqladmin -u <username> -p drop <dbname>`

`mysql -u <username> -p -e "CREATE USER 'user'@'localhost' IDENTIFIED BY 'pass';"`

`mysql -u <username> -p -e "DROP USER 'user'@'localhost';"`

from mysql
----------

`show databases;`

`select user, host from mysql.user;`

`use <dbname>`

`show tables;`

`show tables like "%users%";`

`describe users;`

`show table status;`
