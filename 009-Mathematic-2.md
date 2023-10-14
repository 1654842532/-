---
title: 009-Mathematic-2
date: 2023-03-06 19:54:01
tags:
categories: [Mathematic]
---

本次笔记相关教材为同济第七版高等数学以及习题全解指南两本书

# 第一章习题总结

要记住以下的转化公式:
$\phi_{(x)}=max\{f_{(x)},g_{(x)}\}=\frac 12[f_{(x)}+g_{(x)}+$
$|f_{(x)}-g_{(x)}|]$
$\psi_{x}=min\{f_{(x)},g_{(x)}\}=\frac 12[f_{(x)}+g_{(x)}-$
$|f_{(x)}-g_{(x)}|]$

看到$\sin x_1(\cos x_1)\pm\sin x_2(\cos x_2)$就要想到和积化差公式
看到$\sin x_1(\cos x_1)\sin x_2(\cos x_2)$就要想到积化和差公式

$(1+x)^a-1$~$ax(x \to 0)$一定要**非常熟练**
$x \to 0: x$~$\sin x$~$\tan x$~$\arcsin x$~$\ln (x+1)$~$e^x-1$
$x \to 0: 1=\cos x$~$\frac 12x^2$


## 求 $\lim_{x \to \alpha} \frac {\sin x-\sin \alpha}{x- \alpha}$

<details>
<summary>展开查看</summary>

解:原式 $=\lim_{x \to \alpha}\frac {\sin (\frac {x+\alpha}2+\frac {x-\alpha}2)-\sin (\frac {x+\alpha}2-\frac {x-\alpha}2)} {x-\alpha}$ <br />

$=\lim_{x \to \alpha}\frac {2\cos (\frac {x+\alpha}2)\sin(\frac {x-\alpha}2)}{x-\alpha}$ <br />

$=\lim_{x \to \alpha}\cos (\frac {x+\alpha}2)\lim_{x \to \alpha}\frac {\sin (\frac {x-\alpha}2)}{\frac {x-\alpha}2}$ <br />

$=\cos \alpha$ <br />

思路: 利用和差化积公式化简式子 <br />

</details>


## 求$\lim_{x \to 0}\frac {\sqrt{1+\tan x}-\sqrt{1+\sin x}}{x\sqrt{1+\sin ^2x}-x}$

<details>
<summary>展开查看</summary>

解:原式$=\lim_{x \to 0}\frac {(1+\tan x)^{\frac 12}-1-[(1+\sin x)^{\frac 12}-1]}{x(\sqrt{1+\sin^2x}-1)}$ <br />

$=\lim_{x \to 0}\frac {\frac 12\tan x-\frac 12\sin x}{\sin x\frac 12\sin^2x}$ <br />

$=\lim_{x \to 0}\frac {1-\cos x}{\cos x\sin^2x}$ <br />

$=\lim_{x \to 0}\frac {\frac 12x^2}{\sin^2x}$  <br />

$=\frac 12\lim_{x \to 0}(\frac x{\sin x})^2$ <br />

$=\frac 12$ <br />

思路: 利用$(1+x)^a-1$~$ax(x \to 0)$化简式子 <br />

</details>


## 求$\lim_{x \to 0}\frac {e^{3x}-e^{2x}-e^{x}+1}{\sqrt[3]{(1-x)(1+x)}-1}$

<details>
<summary>展开查看</summary>

解:原式=$\lim_{x \to 0}\frac {(e^x-1)(e^{2x}-1)}{(1-x^2)^{\frac 13}-1}$ <br />

$=\lim_{x \to 0}\frac {2x·x}{\frac 13(-x^2)}$ <br />

$=-6$ <br />

思路: 分母利用因式分解，分子利用$(1+x)^a-1$~$ax(x \to 0)$ <br />

</details>


## 证明:

**任一最高次幂的指数为奇数的代数方程**
**$a_0x^{2n+1}+a_1x^{2n}+\cdots +a_{2n+1}=0$**
至少有一个实根，其中$a_0,a_1,\cdots ,a_{2n+1}$均为常数,$n\in N$

<details>
<summary>展开查看</summary>

证: 当x的绝对值充分大时,$a_0x^{2n+1}+a_1x^{2n}+\cdots +a_{2n+1}$的符号取决于$a_0$的符号，即当x为正时，$f_x$与$a_0$同号,x为负时,$f_x$与$a_0$异号，而$a_0\neq 0$. <br />
因$f_x$是连续函数，它在某充分大的区间的两端处异号,由零点定理可知它在区间内某一点处必定为0，故方程$f_{(x)}=0$至少有一实根 <br />

</details>

## (重要,常见的同阶无穷小)求 $\lim_{x \to 0}\frac {2^x+3^x-2}{x}$

<details>
<summary>展开查看</summary>

解:原式=$\lim_{x \to 0}(\frac {2^x-1}x+\frac {3^x-1}x)$ <br />

令$2^x-1=m$,则$x \to 0$时,$m \to 0$ <br />

$\therefore \lim_{x \to 0}\frac {2^x-1}x$ <br />

$=\lim_{m \to 0}\frac m{\log_2(m+1)}$ <br />

$=\frac 1{\lim_{m \to 0}\frac {\log_2(m+1)}{m}}$ <br />

$=\frac 1{\lim_{m \to 0}\log_2(m+1)^\frac 1m}$ <br />

$=\frac 1{\log_2\lim_{m \to 0}(1+m)^\frac 1m}$ <br />

$=\frac {\log_22}{\log_2e}$ <br />

$=\ln2$ <br />

同理,$\lim_{x\to0}\frac {3^x-1}x=\ln3$ <br />

$\therefore$原式$=\ln2+\ln3$ <br />

</details>

## 面积公式

圆锥表面积$=\pi r^2+\pi rl$
圆锥体积$=\frac 13\pi r^2h$
球表面积$=4\pi r^2$
球体积$=\frac 43\pi r^3$


## 求$\lim_{x \to 0}(\frac {a^x+b^x+c^x}3)^\frac1x(a>0,b>0,c>0)$

<details>
<summary>展开查看</summary>

解:原式$=\lim_{x \to 0}(1+\frac {a^x+b^x+c^x-3}3)^{\frac 3{a^x+b^x+c^x-3}\frac {a^x+b^x+c^x-3}{3x}}$ <br />

$=\lim_{x\to0}e^{\frac {a^x+b^x+c^x-3}{3x}}$ <br />

$=e^{\frac 13\lim_{x\to0}(\frac {a^x-1}x+\frac {b^x-1}x+\frac {c^x-1}x)}$ <br />

$=e^{\frac 13(\ln a+\ln b+\ln c)}$ <br />

$=(abc)^\frac 13$ <br />

思路:配凑以及利用之前求出的常见同阶无穷小 <br />

</details>


## (难)求 $\lim_{x \to \frac \pi2}(\sin x)^{\tan x}$

<details>
<summary>展开查看</summary>

解: 原式$=\lim_{x \to \frac \pi2}[1+(\sin x-1)]^{\frac 1{\sin x-1}(\sin x-1)\tan x}$ <br />

$=e^{\lim_{x\to\frac\pi2}(\sin x-1)\tan x}$ <br />

$\because\lim_{x\to\frac\pi2}(\sin x-1)\tan x$ <br />

$=\lim_{x\to\frac\pi2}\frac{\sin x-\sin\frac\pi2}{\sin(x+\frac\pi2)}\sin x$ <br />

$=\lim_{x\to\frac\pi2}\frac{2\sin(\frac {x-\frac\pi2}2)\cos(\frac {x+\frac\pi2}2)}{2\sin(\frac {x+\frac\pi2}2)\cos(\frac{x+\frac\pi2}2)}\sin x$ <br />

$=\lim_{x\to\frac\pi2}\frac{\sin(\frac x2-\frac\pi4)}{sin(\frac x2+\frac\pi4)}\sin x$ <br />

$=0$ <br />

$\therefore $原式$=e^0=1$ <br />

思路:熟练使用 等量代换、诱导公式、和积化差公式和倍角公式 <br />

</details>


## 易错知识

$f_{(x)}$在$x_0$的某一去心邻域内无界是$\lim_{x\to x_0}f_{(x)}=\infty$的**必要条件**而不是充分条件

比如举个反例: $f_{(x)}=\frac 1{\sin(x-\frac\pi3)}$,$x=\frac\pi3$时，极限为无穷，但是其去心邻域是有界的，就算非常大

