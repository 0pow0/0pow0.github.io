---
title: "Memory"
description: "Memory Virtualization"
math: true
---

![image-20221230183901097](image-20221230183901097.png)



Hardware use base/bound reg to do address translation:

if offset < bound:

Phy Addr = base + offset



## Segmentation

Each logic segmentation (code, stack and heap) assign a pair of base/bound reg to it and complemented with growing direction and permission:

![image-20221230184158281](image-20221230184158281.png)



### Paging

Page table

![image-20221230224657163](image-20221230224657163.png)



Valid bit: whether this translation is valid or not. For example for unallocated page is not valid translation

Protection bit: whether the process has the priviledge to access this page

Present bit: whether this page is in memory or disk

Dirty bit: whether this page has ever been modified since last swapped into memory

![image-20221230231308704](image-20221230231308704.png)



## TLB

![image-20221230234341920](image-20221230234341920.png)

![image-20221230234352300](image-20221230234352300.png)

Use ASID to distinguish different process



### Segmentaion + Paging



![image-20221231000007266](image-20221231000007266.png)



![image-20221231122643032](image-20221231122643032.png)

