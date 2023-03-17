---
title: "Thread"
date: "2022-12-31"
description: "Thread"
math: true
---

# Locks

Hardware primitives:

1. Test-and-set

Pseudo C code:

![image-20230101004939404](image-20230101004939404.png)



With the help of atomic *test-and-set* from hardware, simplest lock implementation would be **spin-lock**

Cons: not working on single CPU, since thread will spin on the while loop and thus owner of the lock get no chance to release this lock.

![image-20230101004617550](image-20230101004617550.png)

