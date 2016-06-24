---
title: Useful Unix Commands
layout: appleII
---

git
---

`git status`

`git remote -v`

`git add UsefulUnixCommands.html`

`git commit -m "add UsefulUnixCommands.html"`

`git push -u origin master`

`git mv UsefulUnixCommands.html UsefulCommands.html`

`git diff`

`git log`

`git log -p -1`

`git config --global log.date iso`

`git update-index --assume-unchanged FILE`

Github
------

`git remote set-url origin git@github.com:davejagoda/davejagoda.github.io.git`

`curl -H X-GitHub-OTP:123456 -u davejagoda https://api.github.com/user/repos`

`curl -d '{"name": "new repo"}' -H X-GitHub-OTP:123456 -u davejagoda https://api.github.com/user/repos`

ssh
---

`ssh-keygen -t rsa -C `uname -n``

`ssh-keygen -p -f ~/.ssh/id_rsa`

`ssh-add`

python
------

`python -i script.py`

ruby
----

`bundle install --path vendor/bundle`

`bundle exec jekyll s`

unix
----

`find -x / -newer /tmp/marker > /tmp/changedfiles.txt`

`grep -Ri searchstring . 2> /tmp/err > /tmp/out`

`grep -r ' $' *`

`grep -r '^ ' *`

`curl -kvI https://www.google.com`

`ntpdc -c sysinfo`

OS X
----

`mdutil -a -i off`

`mdutil -a -i on`

`networksetup -setairportpower en1 off`

`networksetup -setairportpower en1 on`

`systemsetup -getnetworktimeserver`

`diskutil list`

`diskutil info disk0`

`diskutil info disk0s1`

`diskutil info disk0s2`

`mdls photo.jpg`

`plutil -convert xml1 -o - file.plist`

`system_profiler SPStorageDataType`

`systemsetup -gettimezone`

Ubuntu
------

`sudo apt-get update`

`sudo apt-get upgrade`

`sudo apt-get dist-upgrade`

`sudo apt autoremove`
