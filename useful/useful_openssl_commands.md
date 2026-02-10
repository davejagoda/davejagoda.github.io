---
title: Useful OpenSSL commands
layout: appleII
---
```
echo "GET / HTTP/1.0" | openssl s_client -connect davejagoda.github.io:443 > github.cert

openssl x509 -in github.cert -text

openssl genrsa -out private.key 1024

openssl req -new -x509 -key private.key -out publickey.cer -not_before 20260201000000Z -not_after 20260301000000Z -set_serial 0
```
