---
title: "The Weak Law of Large Numbers"
math: true
---

## Markov inequality

> if X > 0 and E[X] is small, then X is unlikely to be very large

markov 给出了RV大于某个值的概率的上界

if $X \geq 0$ and $a > 0$, then $P(X>a) \leq \frac{E[X]}{a}$



## Chebyshev inequality

> if the variance is small, then X is unlikely to be too far from the mean

chebyshev 不等式给出了偏差大于等于某个值的概率的上界

$P(|X-E[X]| \geq \epsilon) \leq \frac{Var(X)}{\epsilon^2}$



## The Weak Law of Large Numbers

