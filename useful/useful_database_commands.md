---
title: Useful database commands
layout: appleII
---

| MySQL              | Oracle                              | Postgres                   | SQLite     |
|--------------------|-------------------------------------|----------------------------|------------|
| SHOW TABLES;       | SELECT table_name FROM user_tables; | \dt+                       | .schema    |
| \q                 | EXIT                                | \q                         | .quit      |
| SELECT DATABASE(); | SELECT * FROM v$database;           | SELECT current_database(); | .databases |
