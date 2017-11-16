---
title: Useful MySQL commands
layout: appleII
---

from command line
-----------------

`mysqld --datadir ~/db/mysql5.7`

`mysqladmin -u root -p shutdown`

`mysql <dbname> -u <username> -p`

`mysql <dbname> -u <username> -p<password>`

`mysqladmin -u <username> -p create <dbname>`

`mysqladmin -u <username> -p drop <dbname>`

from mysql
----------

`show databases;`

`select user, host from mysql.user;`

`use <dbname>`

`show tables;`

`show tables like "%users%";`

`describe users;`
