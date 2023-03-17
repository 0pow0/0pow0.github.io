---
title: "I/O"
description: "I/O"
math: true
---

CPU 和 I/O 设备交互的方式有：polling, Interrupt

快的设备用：polling

慢的设备用：Interrupt

>  Thus, if a device is fast, it may be best to poll; if it is slow, interrupts, which allow overlap, are best. If the speed of the device is not known, or sometimes fast and sometimes slow, it may be best to use a **hybrid** that polls for a little while and then, if the device is not yet finished, uses interrupts. This **two-phased** approach may achieve the best of both worlds.



DMA (Direct Memory Access)

![Cause DMA](dma.png)

怎么去除 `c`: CPU copy data from memory to device

Ans: Use an DMA Engine to do this tedius job

![image-20221228171400171](image-20221228171400171.png)

![iShot_2022-12-28_17.29.43](iShot_2022-12-28_17.29.43.jpg)

# Hard Disk Drive

![image-20221228180420408](image-20221228180420408.png)



![image-20221228181440974](image-20221228181440974.png)
$$
T_{I/O} = T_{seek} + T_{rotation}+T_{transfer}
$$

## RAID

RAID Level 0: 没有备份

:white_check_mark: Performance

:white_check_mark: Capacity

:negative_squared_cross_mark: Reliability

![image-20221228195726827](image-20221228195726827.png)

RAID 1: Mirroring

![image-20221228200059458](image-20221228200059458.png)

每块盘增加一块备份盘

RAID 4: Parity 增加奇偶校验盘

![image-20221228200156576](image-20221228200156576.png)

问题：比如同时修改`block 4` 和`block 13`时，需要更新`P1`和`P3`

，但是`P1`和`P3`在同一盘上，不能sitmultaneously地进行

RAID 5: Rotating Parity![image-20221228200400335](image-20221228200400335.png)
