---
title: Useful OpenSSL Commands
layout: appleII
---

`echo "GET / HTTP/1.0" | openssl s_client -connect davejagoda.github.io:443 > /tmp/github.cert`

`openssl x509 -in /tmp/github.cert -text`
