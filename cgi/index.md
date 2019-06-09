---
title: cgi
layout: default
---

common gateway interface
========================

CGI
---

This is the original approach to making a dynamic website. Each
connection requesting a page that is not static causes a process to
get forked to build the page. The environment is typically used to
pass variables from the web server to the CGI program. STDIN is used
to pass request data to the CGI program, and the program will use
STDOUT to send the response back to the web server.

Bibliography
------------

[RFC3875](https://tools.ietf.org/html/rfc3875)