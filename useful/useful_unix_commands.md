---
title: Useful Unix commands
layout: appleII
---

ssh
---

```
ssh-keygen -t rsa -C $(uname -n)

ssh-keygen -y -f ~/.ssh/id_rsa

ssh-keygen -p -f ~/.ssh/id_rsa

ssh-add
```

python
------

```
python -i script.py
```

ruby
----

```
bundle install --path vendor/bundle

bundle exec jekyll s
```

unix
----

```
find -x / -newer /tmp/marker > /tmp/changedfiles.txt

grep -Ri searchstring . 2> /tmp/err > /tmp/out

grep -r ' $' *

grep -r '^ ' *

curl -kvI https://www.google.com

ntpdc -c sysinfo

TZ=UTC touch -t 197001010000 /tmp/marker

stat /tmp/marker
```

OS X
----

```
dot_clean

mdutil -a -i off

mdutil -a -i on

networksetup -setairportpower en0 off

networksetup -setairportpower en0 on

networksetup -listpreferredwirelessnetworks en0

networksetup -listallhardwareports

systemsetup -getnetworktimeserver

diskutil list

diskutil info disk0

diskutil info disk0s1

diskutil info disk0s2

mdls photo.jpg

plutil -convert xml1 -o - file.plist

system_profiler SPStorageDataType

systemsetup -gettimezone
```

Ubuntu
------

```
sudo apt-get update

sudo apt-get upgrade

sudo apt-get dist-upgrade

sudo apt autoremove
```
