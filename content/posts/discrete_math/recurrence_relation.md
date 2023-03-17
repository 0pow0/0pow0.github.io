---
title: "Recurrence Relations"
date: "2022-12-27"
math: true
---

## First-Order Recurrence Relations: ${a_n = sa_{n-1} + t}$

$a_n$ has this form: $a_n = c_1s^n+c_2$, $c_1, c_2$ solved by
$$
a_0 = c_1+c_2\newline
a_1 = c_1s+c_2
$$




## Second-Order Recurrence Relations: ${a_n = s_1a_{n-1} + s_2a_{n-2}}$

Case 1: $x^2 - s_1x - s_2 = 0$ has **2** root

$a_n$ has this form $a_n = c_1r_1^n+ c_2r_2^n$, where $r_1, r_2$ is the roots. $c_1, c_2$ solved by
$$
a_0 = c_1+c_2 \newline
a_1 = c_1r_1+ c_2r_2
$$


Case 1: $x^2 - s_1x - s_2 = 0$ has **1** root

$a_n$ has this form: $a_n = c_1r^n + c_2nr^n$, where $r$ is the root. $c_1, c_2$ solved by
$$
a_0 = c_1 \newline
a_1 = c_1r+c_2r
$$

