---
title: git push web
layout: appleII
---

git push web
============

On the server
-------------

* Assume two accounts on the server (adjust names as appropriate and
  create if needed)

  1. `user` - the acccount that you will use to ssh and to hold the
     server's copy of the git repository - files under the `user`
     account should **not** be served by the HTTP server

  1. `www` - the account that holds the top level document root

On the client
-------------

* Configure ssh `authorized_keys` such that `ssh web` from the client
  works without prompting for a password

* Create a bare git repository for each site:
```
ssh web 'mkdir production.git && cd production.git && git init --bare'

ssh web 'mkdir staging.git && cd staging.git && git init --bare'
```

* Create a git hook for each site:
```
ssh web 'printf "#!/bin/sh -x\nexport GIT_WORK_TREE=~www/production\ngit checkout -f\ngit clean -df\n" > production.git/hooks/post-receive && chmod +x production.git/hooks/post-receive'

ssh web 'printf "#!/bin/sh -x\nexport GIT_WORK_TREE=~www/staging\ngit checkout -f\ngit clean -df\n" > staging.git/hooks/post-receive && chmod +x staging.git/hooks/post-receive'
```

* Create a remote for each site:
```
git remote add production web:production.git

git remote add staging web:staging.git
```

* Push to each site:
```
git push production production

git push staging staging
```

Bibliography
------------
[Managing a website using git](https://danielmiessler.com/study/git/#website)

[Using git to manage a web site](https://toroid.org/git-website-howto)

[A simple git deployment strategy for static sites](http://nicolasgallagher.com/simple-git-deployment-strategy-for-static-sites/)
