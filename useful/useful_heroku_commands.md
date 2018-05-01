---
title: Useful Heroku commands
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

`heroku releases -a targetapp`

`heroku fork --from sourceapp --to targetapp`

`heroku create -a targetapp`

`heroku destroy -a targetapp`

regions
-------
`heroku regions`

`heroku regions --common`

`curl -n -X GET https://api.heroku.com/regions/us -H "Accept: application/vnd.heroku+json; version=3"`

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

keys
----
`heroku keys`

`heroku keys:add`

local
-----
`heroku local`

`heroku local web`

login
-----
`heroku login`

`export HEROKU_ORGANIZATION=your_organization`

`heroku login --sso`

`heroku whoami`

addons
------
`heroku addons:create papertrail:choklad --name papertrail-targetapp -a targetapp`

postgres
--------
`heroku pg`

`heroku pg:info`

`heroku pg:psql`

`heroku pg:psql -r production COLOR`

`heroku pg:promote COLOR`

django
------
`heroku run python manage.py createsuperuser`

`heroku run python manage.py migrate`

`heroku run python manage.py check`

`heroku run python manage.py dumpdata [app_label.ModelName]`

`heroku run python manage.py shell -c 'from django.contrib.auth.models import User; print(User.objects.make_random_password())'`
