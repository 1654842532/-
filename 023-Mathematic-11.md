---
title: 023-Mathematic-11
date: 2023-03-26 19:03:09
tags:
categories: [Mathematic]
---

本次笔记相关教材为同济第七版高等数学上册以及习题全解指南两本书

# 第五章习题总结

首先，我们要知道:

定积分和不定积分，二者之间的唯一通道是牛顿-莱布尼茨公式

**定积分与不定积分的定义完全不同！**

## 设$f(x)$在[a,b]上连续，在(a,b)内可导，且$f'(x)\leq0.F(x)=\frac1{x-a}\int_a^xf(t)dt$.<br/>证明:在(a,b)内有$F'(x)\leq0$

<details>
<summary>解析</summary>

证:
<br/><br/>

$F'(x)=-\frac1{(x-a)^2}\int_a^xf(t)dt+\frac1{x-a}f(x)$
<br/><br/>

$=-\frac1{(x-a)}f(\xi)+\frac1{x-a}f(x)\:\:\:(\xi\in(a,x)\subset(a,b))$
<br/><br/>

$=\frac1{(x-a)^2}[(x-a)f(x)-(x-a)f(\xi)]$
<br/><br/>

$=\frac{x-\xi}{x-a}f'(\eta)\:\:\:(\eta\in(\xi,x)\subset(a,b))$
<br/><br/>

$\because f'(\eta)\leq0, \therefore F'(x)\leq0$
<br/><br/>

证毕
<br/><br/>

</details>

## 证明: $\int_0^1x^m(1-x)^ndx=\int_0^1x^n(1-x)^mdx\:\:(m,n\in N)$

<details>
<summary>解析</summary>

证:
<br/><br/>

令$x=1-u$,则:
<br/><br/>

$\int_0^1x^m(1-x)^ndx=\int_1^0-(1-u)^mu^ndu$
<br/><br/>

$=\int_0^1x^n(1-x)^mdx$
<br/><br/>

证毕
<br/><br/>

</details>

## 设$f(x)$在[0,1]上连续，$n\in Z$，证明:<br/>$\int_{\frac n2\pi}^{\frac{n+1}2\pi}f(|\sin x|)dx=\int_{\frac n2\pi}^{\frac{n+1}2\pi}f(|\cos x|)dx=\int_0^{\frac\pi2}f(\sin x)dx$

<details>
<summary>解析</summary>

证:
<br/><br/>

令$x=u+\frac n2\pi,$则$dx=du$,因此:
<br/><br/>

$\int_{\frac n2\pi}^{\frac{n+1}2\pi}f(|\sin x|)dx$
<br/><br/>

$=\int_0^{\frac\pi2}f(|\cos(u+\frac n2\pi)|)du$
<br/><br/>

$=\begin{cases}\int_0^{\frac\pi2}f(\sin u)du,&n为偶数,\\\\\int_0^{\frac\pi2}f(\cos u)du,&n为奇数\end{cases}$
<br/><br/>

$\int_{\frac n2\pi}^{\frac{n+1}2\pi}f(|\cos x|)dx$
<br/><br/>

$=\int_0^{\frac\pi2}f(|\cos(u+\frac n2\pi)|)du$
<br/><br/>

$=\begin{cases}\int_0^{\frac\pi2}f(\cos u)du ,&n为偶数\\\\\int_0^{\frac\pi2}f(\sin u)du,&n为奇数\end{cases}$
<br/><br/>

由于$\int_0^{\frac\pi2}f(\sin x)dx=\int_0^{\frac\pi2}f(\cos x)dx.$因此结论成立
<br/><br/>

证毕
<br/><br/>

</details>

## 若$f(t)$是连续的奇函数，证明$\int_0^xf(t)dt$是偶函数；<br/>若$f(t)$是连续的偶函数，证明$\int_0^xf(t)dt$是奇函数


<details>
<summary>解析</summary>

证:
<br/><br/>

记$F(x)=\int_0^xf(t)dt$,则有:
<br/><br/>

$F(-x)=\int_0^{-x}f(t)dt$
<br/><br/>

$\overset{t=-u}{=}\:\:\:-\int_0^xf(-u)du$,
<br/><br/>

当$f(t)$为奇函数时，$F(-x)=\int_0^xf(u)du=F(x)$
<br/><br/>

故$\int_0^xf(t)dt$是偶函数;
<br/><br/>

当$f(t)$为偶函数时，$F(-x)=-\int_0^xf(u)du=-F(x)$
<br/><br/>

故$\int_0^xf(t)dt$是奇函数
<br/><br/>

证毕
<br/><br/>

</details>

## 求定积分:<br/>$J_m=\int_0^\pi x\sin^mxdx\:\:(m\in N_+)$

<details>
<summary>解析</summary>

解:
<br/><br/>

$J_m=\int_0^\pi x\sin^mxdx=\frac\pi2\int_0^\pi\sin^mxdx$
<br/><br/>

而$\int_0^\pi\sin^mxdx$
<br/><br/>

$\overset{x=\frac\pi2+t}{=}\int_{-\frac\pi2}^{\frac\pi2}\cos^mtdt$
<br/><br/>

$=2\int_0^{\frac\pi2}\cos^mtdt$
<br/><br/>

$=2\int_0^{\frac\pi2}\sin^mxdx$
<br/><br/>

$\therefore J_m=\pi\int_0^{\frac\pi2}\sin^mxdx$
<br/><br/>

$=\begin{cases}\frac{2\cdot4\cdot6\cdot\cdots\cdot(m-1)}{1\cdot3\cdot5\cdot\cdots\cdot m}\cdot\pi,&m为大于1的奇数,\\\\\frac{1\cdot3\cdot5\cdot\cdots\cdot(m-1)}{2\cdot4\cdot6\cdot\cdots\cdot m}\cdot\frac{\pi^2}2,&m为偶数\end{cases}$
<br/><br/>

$J_1=\pi$
<br/><br/>

</details>

## 用$\Gamma$函数表示下面的积分，并指出这个积分的收敛范围<br/>$\int_0^1(\ln\frac1x)^pdx$

<details>
<summary>解析</summary>

解:
<br/><br/>

$\because\Gamma(p)=\int_0^{+\infty}e^{-x}x^{p-1}dx$
<br/><br/>

令$x=\ln\frac1u,\:\:\therefore dx=-\frac1udu,\:\:u=e^{-x}$
<br/><br/>

$\therefore\Gamma(p)=\int_1^{0^+}u\cdot(\ln\frac1u)^{p-1}(-\frac1u)du$
<br/><br/>

$=\int_0^1(\ln\frac1x)^{p-1}dx$
<br/><br/>

$\therefore\int_0^1(\ln\frac1x)^pdx=\Gamma(p+1)$
<br/><br/>

当$p> -1$时，积分收敛
<br/><br/>

</details>






