---
title: README
layout: appleII
---

Install and run locally
=======================

```
bundle install
bundle exec jekyll serve --incremental &
```

Check index.md freshness
========================

```
diff \
<(grep '\[' index.md | cut -d \[ -f 2 | cut -d \] -f 1 | sort) \
<(find . -type d -maxdepth 1 | sort | cut -d / -f 2 | sort)
```
