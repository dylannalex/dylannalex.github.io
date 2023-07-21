---
title: Random Circle Problem
date: 2023-07-21 13:42:57
categories: [Math Topics]
tags: [probability, english]
math: true
permalink: /random_circle_problem/
img_path: ../assets/img/posts/2023-07-21-random_circle/
---

Test your logic and probability skills with this simple problem. Try to solve it before reading the solution!

## Statement

Given a circle $C_a$ of radius $a$ fully contained in a square $S$ of side $a$

![png](statement.png){: w="500" h="500"}

Now, consider randomly choosing a circle $C_b$ with radius $b$ (where $0 < b < a$) inside the same square $S$. What is the probability that $C_b$ is entirely contained within $C_a$?


## Solution

Let's think of a random point $P$ inside the square $S$. Then, the circle $C_b$ is described by the circumference of radius $b$ centered at $P$. If $C_b$ is fully contained in $C_a$, then the distance between $P$ and the circumference of $C_a$ must be greater than $b$.

![png](step1.png){: w="500" h="500"}

This means that $C_b$ is fully contained in $C_a$ if and only if its center $P$ is inside the circle $C_{ab}$ of radius $a-b$ with the same center as $C_a$.

![png](step2.png){: w="500" h="500"}

Then the probability that $C_b$ is fully contained in $C_a$ is the ratio between the area of $C_{ab}$ and the area of $S$:

$$
\mathbb{P}(C_b \text{ fully contained in } C_a) = \frac{\pi (a-b)^2}{a^2}
$$