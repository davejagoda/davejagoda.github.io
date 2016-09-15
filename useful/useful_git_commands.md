---
title: Useful Git Commands
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

`git fetch`

`git rebase`

`git branch -a`

`git checkout feature/frobnicate`

`git checkout -b feature/frobnicate-dj`

`git push -u origin feature/frobnicate-dj`

`git rebase -i HEAD~1`

`git commit --amend`

`git rebase --continue`

Github
------

`git remote set-url origin git@github.com:davejagoda/davejagoda.github.io.git`

`curl -H X-GitHub-OTP:123456 -u davejagoda https://api.github.com/user/repos`

`curl -d '{"name": "new repo"}' -H X-GitHub-OTP:123456 -u davejagoda https://api.github.com/user/repos`
