---
title: 021-Mathematic-9
date: 2023-03-22 21:24:50
tags:
categories: [Mathematic]
---

# 第四章习题总结

## 求不定积分: $\int\frac{dx}{3+\sin^2x}$

<details>
<summary>解析</summary>
解:原式
<br/><br/>

$=\int\frac{\csc^2xdx}{3\csc^2x+1}$
<br/><br/>

$=-\int\frac{d(\cot x)}{3\csc^2x+1}$
<br/><br/>

$=-\int\frac{d(\cot x)}{3\cot^2x+4}$
<br/><br/>

$=-\frac13\int\frac{d(\cot x)}{(\frac2{\sqrt{3}})^2+\cot^2x}$
<br/><br/>

$=-\frac13\cdot\frac{\sqrt{3}}2\arctan(\frac{\sqrt{3}}2\cot x)+C$
<br/><br/>

思路: 一时难以简单转化$sin^2x$,所以将其转换为$\csc^2x$.然后要利用好$\cot^2x+1=\csc^2x$这个公式，这个公式不容易想起来，但是此题很实用
<br/><br/>

</details>

## 求不定积分: $\int\frac{x+\sin x}{1+\cos x}dx$

<details>
<summary>解析</summary>

解:原式
<br/><br/>

$=\int\frac{x+\frac{2\tan\frac x2}{1+\tan^2x}}{1+\frac{1-\tan^2\frac x2}{1+\tan^2\frac x2}}dx$
<br/><br/>

$=\int\frac x2\sec^2\frac x2dx+\int\tan\frac x2dx$
<br/><br/>

$=\int xd(\tan\frac x2)+\int\tan\frac x2d(x)$
<br/><br/>

$=x\cdot\tan\frac x2+C$
<br/><br/>

思路: 万能公式+分部积分逆运用
<br/><br/>

</details>

## 求不定积分: $\int\frac{e^{3x}+e^x}{e^{4x}-e^{2x}+1}dx$

<details>
<summary>解析</summary>

解:原式
<br/><br/>

$=\int\frac{e^x+e^{-x}}{e^{2x}-1+e^{-2x}}dx$
<br/><br/>

$=\int\frac{d(e^x-e^{-x})}{(e^x-e^{-x})^2+1}$
<br/><br/>

$=\arctan(e^x-e^{-x})+C$
<br/><br/>

思路: 首先分子分母同时除以$e^{2x}$，目的是为了能够将分子配凑出与分母相适应的微分等式，本题配凑巧妙，所以记录下来
<br/><br/>

</details>

## 求不定积分: $\int\frac{\sin x\cos x}{\sin x+\cos x}dx$

<details>
<summary>解析</summary>

解法一:
<br/><br/>

解：原式
<br/><br/>

$=\int\frac{\sin x\cos x}{\sqrt{2}\sin(x+\frac\pi4)}dx$
<br/><br/>

令$u=x+\frac\pi4$
<br/><br/>

则原式
<br/><br/>

$=\int\frac{2\sin^2u-1}{2\sqrt{2}\sin u}du$
<br/><br/>

$=\frac{1}{\sqrt{2}}\int\sin udu-\frac1{2\sqrt{2}}\int\csc udu$
<br/><br/>

$=-\frac{\cos(x+\frac\pi4)}{\sqrt{2}}-\frac1{2\sqrt{2}}\ln|\csc(x+\frac\pi4)-\cot(x+\frac\pi4)|+C$
<br/><br/>

解法二:
<br/><br/>

解：原式
<br/><br/>

$=\int\frac{\frac12(\sin x+\cos x)^2-\frac12}{\sin x+\cos x}dx$
<br/><br/>

$=\frac12\int(\sin x+\cos x)dx-\frac12\int\frac1{\sin x+\cos x}dx$
<br/><br/>

$\frac12(-\cos x+\sin x)-\frac12\int\frac1{\sin x+\cos x}dx$
<br/><br/>

令$u=\tan\frac x2$则$\sin x=\frac{2u}{1+u^2}, \cos x=\frac{1-u^2}{1+u^2}$
<br/><br/>

$dx=\frac2{1+u^2}du$,故有:
<br/><br/>

$\int\frac1{\sin x+\cos x}dx=\int\frac2{2u+1-u^2}$
<br/><br/>

$=-\int\frac2{(u-1)^2-(\sqrt{2})^2}du$
<br/><br/>

$=-\frac1{\sqrt{2}}\int\frac1{u-1-\sqrt{2}}du+\frac{1}{\sqrt{2}}\int\frac1{u-1+\sqrt{2}}du$
<br/><br/>

$=\frac1{\sqrt{2}}\ln|\frac{u-1+\sqrt{2}}{u-1-\sqrt{2}}|+C'$
<br/><br/>

因此有:
<br/><br/>

$\int\frac{e^{3x}+e^x}{e^{4x}-e^{2x}+1}dx=\frac12(\sin x-\cos x)-\frac1{2\sqrt{2}}\ln|\frac{\tan\frac x2-1+\sqrt{2}}{\tan\frac x2-1+\sqrt{2}}|+C$
<br/><br/>

思路:解法一使用了辅助角公式和换元积分法
<br/><br/>

解法二使用了万能公式进行积分
<br/><br/>

</details>
