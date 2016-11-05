---
title: Useful Heroku Commands
layout: appleII
---

apps
----

`heroku apps`

`heroku apps -A`

`heroku apps:info`

`heroku apps:info -a davejagoda`

`heroku apps:info -a davejagoda-staging`

`heroku apps:info -r production`

`heroku apps:info -r staging`

remotes
-------

`heroku git:remote -a davejagoda -r production`

`heroku git:remote -a davejagoda-staging -r staging`

`git push production`

`git push staging`

config
------

`heroku config`

`heroku config:set SECRET_KEY=u'<SECRET_STUFF>'`

`heroku config:unset SECRET_KEY`

local
-----

`heroku local`

`heroku local web`

postgres
--------

`heroku pg`

`heroku pg:psql`

`heroku pg:psql -r production cobalt`

django
------

`heroku run python manage.py createsuperuser`

`heroku run python manage.py migrate`
