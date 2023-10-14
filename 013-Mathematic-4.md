---
title: 013-Mathematic-4
date: 2023-03-08 15:39:23
tags:
categories: [Mathematic]
---

本次笔记相关教材为同济第七版高等数学以及习题全解指南两本书

# 第二章习题总结

要 ***牢记*** 31个基本公式以及导数公式

要 ***牢记*** 6个初等函数的n阶导数

要 ***牢记*** 莱布尼茨公式以及一些基本排列组合公式

## 计算下列各根式的近似值

$(1)\sqrt[3]{996}; (2)\sqrt[6]{65}$

<details>
<summary>展开查看</summary>

解: 由$\sqrt[n]{1+x}\approx1+\frac xn$知 <br/>

$(1) \sqrt[3]{996}=\sqrt[3]{1000-4}=10\sqrt[3]{1-\frac4{1000}}$ <br/>
$\approx10[1+\frac13(-\frac4{1000})]\approx9.987$ <br/>

$(2) \sqrt[6]{65}=\sqrt[6]{64+1}=2\sqrt[6]{1+\frac1{64}}$ <br/>
$\approx2(1+\frac16\cdot\frac1{64})\approx2.0052$ <br/>

</details>

## 选出一个正确的结论

设$f_{(x)}$在$x=a$的某个邻域内有定义，则$f_{(x)}$在$x=a$处可导的一个充分条件是():

$(A) \lim_{h\to+\infty}h[f_{(a+\frac1h)}-f_{(a)}]$存在

$(B) \lim_{h\to0}\frac {f_{(a+2h)}-f_{(a+h)}}h$存在

$(C) \lim_{h\to0}\frac{f_{(a+h)}-f_{(a-h)}}{2h}$存在

$(D) \lim_{h\to0}\frac{f_{(a)}-f_{(a-h)}}h$存在

<details>
<summary>解析</summary>

思路: 本题的关键在于: 只要**极限中没有出现$f_{(a)}$**,那么就存在漏洞。<br/>
问题就在于当$f_{(a)}$正巧是函数$f_{(x)}$的**分段函数点**的时候，没有$f_{(a)}$存在的式子必然会一边导向一个函数，另一边导向另一个函数，这样结果肯定是错的<br/>

解: (A)只能得出右极限，因为是$h\to+\infty$的情况 <br/>

(B)取$f_{(x)}=\begin{cases} 1,x≠0 \\\\ 0,\text{x=0} \end{cases}$,此时B显然错误，x=0处是不可导的，但是B却算出导数为0 <br/>

(C)取$f_{(x)}=|x|$，显然x=0处不可导，而C却算出导数为0 <br/>

(D)正确 <br/>

</details>

## 求导数

$y=\ln\tan\frac x2 -\cos x\cdot\ln\tan x$

<details>
<summary>解析</summary>

解: $y'=\frac{\frac12\sec^2\frac x2}{\tan\frac x2}+\sin x\ln\tan x-\cos x\frac{\sec^2x}{\tan x}$ <br/>

$=\frac12\frac1{\sin\frac x2\cos\frac x2}-\frac1{\sin x}+\sin x \ln\tan x$ <br/>

$=\sin x\ln\tan x$ <br/>

</details>

## 总2-14

**已知$f_{(x)}$是周期为5的连续函数，它在x=0的某个邻域内满足关系式**

$f_{(1+\sin x)}-3f_{(1-\sin x)}=8x+o(x)$

**且$f_{(x)}$在$x=1$处可导，求曲线$y=f_{(x)}$在点$(6,f(6))$处的切线方程**

<details>
<summary>解析</summary>

解:<br/>

由$f_{(x)}$连续，令关系式两端$x\to0$,取极限得: <br/>

$f_{(1)}-3f_{(1)}=0$ <br/>

$\therefore f_{(1)}=0$ <br/>

又: <br/>

$\lim_{x\to0}\frac{f(1+\sin x)-3f(1-\sin x)}x=8$ <br/>

而: <br/>

$\lim_{x\to0}\frac{f(1+\sin x)-3f(1-\sin x)}{x}$ <br/>

$=\lim_{x\to0}\frac{f(1+\sin x)-3f(1-\sin x)}{\sin x}\cdot\lim_{x\to0}\frac{\sin x}{x}$ <br/>

令$t=\sin x$ <br/>

则原式$=\lim_{t\to0}\frac{f(1+t)-3f(1-t)}t$ <br/>

$=\lim_{t\to0}\frac{f(1+t)-f(1)}{t}+3\lim_{t\to0}\frac{f(1-t)-f(1)}{-t}$ <br/>

$=4f'(1)$ <br/>

故$f'(1)=2$ <br/>

而$f(x)$是周期为5的函数 <br/>

$\therefore f'(6)=\lim_{x\to0}\frac{f(6+x)-f(6)}x$ <br/>

$=\lim_{x\to0}\frac{f(1+x)-f(1)}{x}=f'(1)=2$ <br/>

$\therefore$切线方程为: $2x-y-12=0$ <br/>

</details>

