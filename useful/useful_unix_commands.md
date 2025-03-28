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

ssh-keygen -l -E md5 -f ~/.ssh/id_rsa.pub

ssh-add
```

perl
----

```
perl -p -i -e 's/this/that/g' *.txt
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
dscl . -list /Users UniqueID | sort -n -k 2

dot_clean

fs_usage

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

ls -ale

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

CentOS
------

```
yum provides java

yum provides python?

yum provides */javac
```

SELinux
-------

```
getenforce

ls -Z

ps -Z
```
