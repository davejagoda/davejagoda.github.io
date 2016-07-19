---
title: assembly language
layout: default
---

Assembly language
=================

This is the lowest level programming that a programmer would typically
ever have to do

The level below this is machine language, which are instructions the
processor can perform

Assembly language typically corresponds one to one with a processing
chip architecture (e.g. Intel x86, ARM, Motorola 680x0, MOS 6502,
SPARC, MIPS)

There are also High Level Assembly languages


Things associated with Assembly language
----------------------------------------

Programs are assembled by an assembler

Perhaps better to call these assembly languages

It's not clear who the original authors are - perhaps each machine
architecture had a programmer that built an assembly language to make
it easier to write code

Assembly languages are still in use today

example program
---------------

from wikipedia

```
adosseg
.model small
.stack 100h

.data
hello_message db 'Hello, World!',0dh,0ah,'$'

.code
main  proc
      mov    ax,@data
      mov    ds,ax

      mov    ah,9
      mov    dx,offset hello_message
      int    21h

      mov    ax,4C00h
      int    21h
main  endp
end   main```

Discussion
----------

What's wrong with assembly language?

![Motorola 6800 Assembly Language](https://upload.wikimedia.org/wikipedia/commons/f/f3/Motorola_6800_Assembly_Language.png)
