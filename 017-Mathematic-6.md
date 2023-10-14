---
title: 017-Mathematic-6
date: 2023-03-13 12:53:53
tags:
categories: [Mathematic]
---

# 第三章习题总结

首先补充说明: 高阶无穷小无所谓正负号，$+o(x)$等价于$-o(x)$,$o(x)+o(x)=o(x)$,$o(x)-o(x)=o(x)$

学完这章之后，个人认为求极限的思路是这样的:

(1)如果原式能够转化为x的幂并且x的高阶无穷小正好跟某一对应的低阶无穷小对齐的话，就要用泰勒展开，否则就尝试第一章的运算法则以及等价无穷小等转换；否则就尝试洛必达法则

(2)当极限的过程为$x\to\infty$时，如果要用泰勒展开，那么展开时就要按$\frac1x$的幂展开并且带上与$\frac1x$有关的高阶无穷小


## 请证明:

**方程$x^5+x-1=0$只有一个正根**

<details>
<summary>解析</summary>

证:<br/>

取函数$f(x)=x^5+x-1,f(x)$在[0,1]上连续,<br/>

$f(0)=-1<0, f(1)=1>0$ <br/>

由零点定理知,至少存在点$x_1\in(0,1),$使$f(x_1)=0$ <br/>

即方程$x^5+x-1=0$在(0,1)内至少有一个正根 <br/>

若该方程还有一个正根$x_2$,即$f(x_2)=0$,则由$f(x)=x^5+x-1$在$[x_1,x_2]$(或$[x_2,x_1]$)上连续，在$(x_1,x_2)$(或$(x_2,x_1)$)内可导，知$f(x)$满足罗尔定理条件<br/>

故至少存在点$\xi\in(x_1,x_2)$(或$(x_2,x_1)$)使:<br/>

$f'(\xi)=0$ <br/>

但$f'(\xi)=5\xi^4+1>0$,矛盾 <br/>

因此，该方程只有一个正根<br/>

证毕<br/>

</details>

## 请证明:

**若函数$f(x)$在$(-\infty,+\infty)$内满足关系式$f'(x)=f(x),且f(0)=1,$则$f(x)=e^x$**

<details>
<summary>解析</summary>

证:<br/><br/>

取函数$F(x)=\frac{f(x)}{e^x},$ <br/><br/>

$\because F'(x)=\frac{f'(x)e^x-f(x)e^x}{e^{2x}}$ <br/><br/>

$=\frac{f'(x)-f(x)}{e^x}$ <br/><br/>

$=0$<br/><br/>

故$F(x)=C$.又$F(0)=C=f(0)=1$ <br/><br/>

因此$F(x)=1$ <br/><br/>

故$f(x)=e^x$ <br/><br/>

</details>

## 利用泰勒公式求下列极限:

(1) $\lim_{x\to+\infty}(\sqrt[3]{x^3+3x^2}-\sqrt[4]{x^4-2x^3})$

<details>
<summary>解析</summary>

解: <br/><br/>

令$f(\frac1x)=(1+\frac1x)^{\frac13}$,则由$\frac1x$的幂展开带佩亚诺余项的1阶泰勒公式为:<br/><br/>

$f(\frac1x)=f(0)+f'(0)\frac1x+o(\frac1x)$ <br/><br/>

$=1+\frac13\cdot3\cdot\frac1x+o(\frac1x)=1+\frac1x+o(\frac1x)$<br/><br/>

令$f(\frac1x)=(1-\frac2x)^{\frac14}$,则由$\frac1x$的幂展开带佩亚诺余项的1阶泰勒公式为:<br/><br/>

$f(\frac1x)=f(0)+f'(0)\frac1x+o(\frac1x)$<br/><br/>

$=1-\frac14\cdot2\cdot\frac1x+o(\frac1x)=1-\frac1{2x}+o(\frac1x)$<br/><br/>

$\therefore$原式=$\lim_{x\to+\infty}x[1+\frac1x+o(\frac1x)-1+\frac1{2x}-o(\frac1x)]$<br/><br/>

$=\lim_{x\to+\infty}\frac32+\frac{o(\frac1x)}{\frac1x}=\frac32$<br/><br/>

</details>

(2) $\lim_{x\to0}\frac{\cos x-e^{-\frac{x^2}2}}{x^2[x+\ln(1-x)]}$

<details>
<summary>解析</summary>

解: <br/><br/>

原式=$\lim_{x\to0}\frac{1-\frac{x^2}{2}+\frac{x^4}{4!}+o(x^4)-1-(-\frac{x^2}{2})-\frac12(-\frac{x^2}{2})^2+o(x^4)}{x^2[x+(-x-\frac12x^2+o(x^2))]}$ <br/><br/>

$=\lim_{x\to0}\frac{(\frac1{4!}-\frac18)x^4+o(x^4)}{-\frac12x^4+o(x^4)}$<br/><br/>

$=\lim_{x\to0}\frac{-\frac1{12}+\frac{o(x^4)}{x^4}}{-\frac12+\frac{o(x^4)}{x^4}}$<br/><br/>

$=\frac{-\frac1{12}}{-\frac12}=\frac16$<br/><br/>

</details>

(3) $\lim_{x\to0}\frac{1+\frac12x^2-\sqrt{1+x^2}}{(\cos x-e^{x^2})\sin{x^2}}$

<details>
<summary>解析</summary>

解: 原式$=\lim_{x\to0}\frac{1+\frac12x^2-1-\frac12x^2+\frac18x^4+o(x^4)}{[1-\frac12x^2+o(x^2)-1-x^2+o(x^2)](x^2+o(x^2))}$ <br/><br/>

$=\lim_{x\to0}\frac{\frac18x^4+o(x^4)}{(-\frac32x^2+o(x^2))(x^2+o(x^2))}$<br/><br/>

$=\lim_{x\to0}\frac{\frac18x^4+o(x^4)}{-\frac32x^4-\frac12x^2o(x^2)+o(x^4)}$ <br/><br/>

$=\lim_{x\to0}\frac{\frac18x^4+o(x^4)}{-\frac32x^4+o(x^4)}$ <br/><br/>

$=\lim_{x\to0}\frac{\frac18+\frac{o(x^4)}{x^4}}{-\frac32+\frac{o(x^4)}{x^4}}$ <br/><br/>

$=\frac{\frac18}{-\frac32}=-\frac1{12}$<br/><br/>

</details>

(4) $\lim_{x\to\infty}[x-x^2\ln(1+\frac1x)]$

<details>
<summary>解析</summary>

解: 原式$=\lim_{x\to\infty}[x-x^2(\frac1x-\frac12\cdot\frac1{x^2}+o(\frac1{x^2}))]$ <br/><br/>

$=\lim_{x\to\infty}[x-x+\frac12+\frac{o(\frac1{x^2})}{\frac1{x^2}}]$ <br/><br/>

$=\frac12$ <br/><br/>

</details>


## 请证明:

设I为一无穷区间，函数$f(x)$在I上连续，I内可导，试证明:如果在I的任一有限的子区间上$f'(x)\geq0(或f'(x)\leq0)$,且等号仅在有限多个点处成立，那么$f(x)$在区间I上单调增加(或单调减少)

<details>
<summary>解析</summary>

证: <br/><br/>

在I内任取两点$x_1,x_2$,不妨设$x_1< x_2$,在$[x_1,x_2]$上应用拉格朗日中值定理，得到: <br/><br/>

$f(x_2)-f(x_1)=f'(\xi)(x_2-x_1)\geq0$(或$\leq0$), <br/><br/>

其中$\xi\in(x_1,x_2)$，即$f(x_2)\geq f(x_1)$(或$f(x_2)\leq f(x_1)$) <br/><br/>

因此$f(x)$在I上单调不减(或单调不增) <br/><br/>

从而对任一$x\in[x_1,x_2]$,有: <br/><br/>

$f(x_2)\geq f(x)\geq f(x_1)$ (或$f(x_2)\leq f(x)\leq f(x_1)$) <br/><br/>

若$f(x_1)=f(x_2)$,则有$f(x)\equiv f(x_1), x\in[x_1,x_2]$ <br/><br/>

故$f'(x)\equiv0,x\in[x_1,x_2]$ <br/><br/>

这与$f'(x)=0$在I的任一有限子区间上仅在有限多个点处成立的假定相矛盾 <br/><br/>

因此$f(x_2)>f(x_1)$(或$f(x_2)<f(x_1)$) <br/><br/>

即$f(x)$在区间I上单调增加(或单调减少) <br/><br/>

</details>

## 如题

设$y=f(x)$在$x=x_0$的某邻域内具有三阶连续导数，如果$f''(x_0)=0$,而$f'''(x_0)\neq0$,试问$(x_0,f(x_0))$是否为拐点?为什么? 

<details>
<summary>解析</summary>

解:<br/><br/>

已知$f'''(x_0)\neq0$,不妨设$f'''(x_0)>0$,由于$f'''(x)$在$x=x_0$的某个邻域内连续<br/><br/>

因此必存在$\delta>0$,当$x\in(x_0-\delta,x_0+\delta)$时$f'''(x)>0$<br/><br/>

故在$(x_0-\delta,x_0+\delta)$内$f''(x)$单调增加。<br/><br/>

又已知$f''(x_0)=0$<br/><br/>

从而当$x\in(x_0-\delta,x_0)$时，$f''(x)<f''(x_0)=0$<br/><br/>

即函数$f(x)$在$(x_0-\delta,x_0)$内的图形是凸的<br/><br/>

当$x\in(x_0,x_0+\delta)$时，$f''(x)>f''(x_0)=0$<br/><br/>

即函数$f(x)$在$(x_0,x_0+\delta)$内的图形是凹的<br/><br/>

所以点$(x_0,f(x_0))$为曲线的拐点<br/><br/>

</details>

## 求$\lim_{x\to+\infty}(\frac2\pi\arctan x)^x$

<details>
<summary>解析</summary>

解:原式<br/><br/>

$=e^{\lim_{x\to+\infty}x\cdot\ln(\frac2\pi\arctan x)}$<br/><br/>

而$\lim_{x\to+\infty}x\cdot\ln(\frac2\pi\arctan x)$<br/><br/>

$=\lim_{x\to+\infty}x\cdot(\ln\frac2\pi+\ln\arctan x)$<br/><br/>

$=\lim_{x\to+\infty}\frac{\ln\arctan x-\ln\frac2\pi}{\frac1x}$<br/><br/>

$\overset{洛}{=}\lim_{x\to+\infty}\frac{\frac1{(\arctan x)(1+x^2)}}{-\frac1{x^2}}$<br/><br/>

$=\lim_{x\to+\infty\frac{-1}{\arctan x\cdot(\frac{x^2+1}{x^2})}}$<br/><br/>

$=-\frac2\pi$<br/><br/>

$\therefore$原式$=e^{-\frac2\pi}$<br/><br/>

</details>

## 求$\lim_{x\to\infty}[\frac{(a_1^{\frac1x}+a_2^{\frac1x}+\cdots+a_n^{\frac1x})}n]^{nx}$(其中，$a_1,a_2,\cdots,a_n>0$)

<details>
<summary>解析</summary>

解:原式<br/><br/>

$=\lim_{x\to\infty}(1+\frac{a_1^{\frac1x}-1+a_2^{\frac1x}-1+\cdots+a_n^{\frac1x}-1}n)^{\frac{nx}{a_1^{\frac1x}-1+a_2^{\frac1x}-1+\cdots+a_n^{\frac1x}-1}\cdot(a_1^{\frac1x}+a_2^{\frac1x}+\cdots+a_n^{\frac1x}-n)}$<br/><br/>

$=e^{\lim_{x\to\infty}x(a_1^{\frac1x}+a_2^{\frac1x}+\cdots+a_n^{\frac1x}-n)}$<br/><br/>

而$\lim_{x\to\infty}\frac{a_1^{\frac1x}+a_2^{\frac1x}+\cdots+a_n^{\frac1x}-n}{\frac1x}$<br/><br/>

令$t=\frac1x,x\to\infty,t\to0$<br/><br/>

$\lim_{t\to0}(a_1^t\ln a_1+a_2^t\ln a_2+\cdots+a_n^t\ln a_n)$<br/><br/>

$=\ln(a_1a_2\cdots a_n)$<br/><br/>

$\therefore$原式$=e^{\ln(a_1a_2\cdots a_n)}$<br/><br/>

$=a_1a_2\cdots a_n$<br/><br/>

</details>

## 请证明:

**设$f''(x_0)$存在,证明: $\lim_{h\to0}\frac{f(x_0+h)+f(x_0-h)-2f(x_0)}{h^2}=f''(x_0)$**

<details>
<summary>解析</summary>

证:<br/><br/>

$\lim_{h\to0}\frac{f(x_0+h)+f(x_0-h)-2f(x_0)}{h^2}$<br/><br/>

$\overset{洛}{=}\lim_{x\to0}\frac{f'(x_0+h)+f'(x_0-h)-2f'(x_0)}{2h}$<br/><br/>

$=\frac12\lim_{h \to 0}\frac{f'(x_0+h)-f'(x_0)-(f'(x_0)-f'(x_0-h))}{h}$<br/><br/>

$=\frac12(f''(x_0)+f''(x_0))=f''(x_0)$<br/><br/>

证毕<br/><br/>

</details>

## 请证明:

**设$f(x)$在(a,b)内二阶可导,且$f''(x)\geq0$.证明对于(a,b)内任意两点$x_1,x_2$及$0\leq t\leq1$,有:**

$f[(1-t)x_1+tx_2]\leq(1-t)f(x_1)+tf(x_2)$

<details>
<summary>解析</summary>

证:<br/><br/>

由$x_1,x_2\in(a,b)$知$x_0=(1-t)x_1+tx_2\in(a,b),$利用泰勒公式有:<br/><br/>

$f(x_1)=f(x_0)+f'(x_0)(x_1-x_0)+\frac1{2!}f''(\xi_1)(x_1-x_0)^2$<br/><br/>

$\xi_1$介于$x_1$与$x_0$之间<br/><br/>

$f(x_2)=f(x_0)+f'(x_0)(x_2-x_0)+\frac1{2!}f''(\xi_2)(x_2-x_0)^2$<br/><br/>

$\xi_2$介于$x_2$与$x_0$之间<br/><br/>

由$f''(x)\geq0$知$f''(\xi_1)\geq0,f''(\xi_2)\geq0$,故:<br/><br/>

$f(x_1)\geq f(x_0)+f'(x_0)(x_1-x_0)$<br/><br/>

及$f(x_2)\geq f(x_0)+f'(x_0)(x_2-x_0)$,<br/><br/>

$\therefore (1-t)f(x_1)+tf(x_2)$<br/><br/>

$\geq(1-t)f(x_0)+tf(x_0)+f'(x_0)[(1-t)(x_1-x_0)+t(x_2-x_0)]$<br/><br/>

$=f(x_0)+f'(x_0)[(1-t)x_1+tx_2-x_0]=f(x_0)$<br/><br/>

即$f[(1-t)x_1+tx_2]\leq(1-t)f(x_1)+tf(x_2)$<br/><br/>

证毕<br/><br/>

</details>


