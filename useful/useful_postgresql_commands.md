---
title: Useful PostgreSQL commands
layout: appleII
---

from command line
-----------------

`pg_ctl -D ~/db/postgres9.6 -l ~/db/postgres9.6/logfile start`

`pg_ctl -D ~/db/postgres9.6 stop`

`psql -U postgres`

`createuser`

from psql
---------

`\?`

`\q`

`\l`

`\dn`

`\dn+`

`\c <dbname>`

`\d [<tablename>|<viewname>]`

`\d+ [<tablename>|<viewname>]`

`\dt *.*`

`\du`

`\dv`

`\o /tmp/psql.out`

`\o`

`SELECT current_time;`
