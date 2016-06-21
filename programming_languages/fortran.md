---
title: Fortran
layout: default
---

Fortran
=======

History
-------

The name Fortran is a contraction of Formula Translation

Developed at IBM by John Backus and a team of programmers

Still in use today - the Lindy effect

Considered a high level programming language

Intended as an alternative to [assembly language](assembly) for the IBM 704 mainframe

Example program
---------------

Here is a program in the Fortran 77 dialect:

```fortran
      PROGRAM CENTIGRADE_TO_FAHRENHEIT
      INTEGER C, Z
      REAL R
      PARAMETER (Z = 32)
      PARAMETER (R = 9.0 / 5.0)
      DO 10, C = 0, 40
         F = (C * R) + Z
         WRITE (*, 99) C, F
 99      FORMAT (I2, F6.1)
 10   CONTINUE
      STOP
      END
```

This can be compiled using gcc's gfortran on operating systems like OS X or Linux

Discussion
----------

What's wrong with Fortran?

![FORTRAN Coding Form](https://upload.wikimedia.org/wikipedia/commons/1/18/FortranCodingForm.png)
