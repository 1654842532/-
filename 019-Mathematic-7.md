---
title: 019-Mathematic-7
date: 2023-03-22 13:48:45
tags:
categories: [Mathematic]
toc: true
---

本次笔记相关教材为同济第七版高等数学上册以及习题全解指南两本书

## 4-1: 不定积分的概念与性质

**一、原函数与不定积分的概念**

**定义Ⅰ:**

如果在区间上，可导函数$F(x)$的导函数为$f(x)$,即对任一$x\in I$,都有:

$F'(x)=f(x)$或$dF(x)=f(x)dx$,

那么函数$F(x)$就称为$f(x)$或$f(x)dx$在区间I上的一个原函数

原函数存在定理: 如果函数$f(x)$在区间I上连续，那么在区间I上存在可导函数$F(x)$,使对任一$x\in I$,都有:$F'(x)=f(x)$

简单地说就是： 连续函数一定有原函数

**定义Ⅱ:**

在区间I上，函数$f(x)$的带有任意常数项的原函数称为$f(x)$在区间I上的不定积分，记作 $\int f(x)dx$

其中记号$\int$称为积分号，$f(x)$称为被积函数，$f(x)dx$称为被积表达式，x称为积分变量

注意:

(1). $f(x)$的原函数的图形称为$f(x)$的积分曲线

(2). $\int f(x)dx$的图形是$f(x)$所有积分曲线组成的平行曲线簇

(3). $\frac d{dx}[\int f(x)dx]=f(x)$或$d[\int f(x)dx]=f(x)dx$

说明: 微分运算(以记号d表示)与求不定积分的运算(简称积分运算，以记号$\int$表示)是互逆的。当两个记号连在一起时，或者抵消，或者抵消后差一个常数

**二、基本积分表(重要):**

1. $\int kdx=kx+C$(k为常数)
<br/><br/>

2. $\int x^\mu dx=\frac{x^{\mu+1}}{\mu+1}+C(\mu\neq-1)$
<br/><br/>

3. $\int \frac{dx}x=\ln|x|+C$
<br/><br/>

4. $\int\frac{dx}{1+x^2}=\arctan x+C$或$-arccotx+C$
<br/><br/>

5. $\int\frac{dx}{\sqrt{1-x^2}}=\arcsin x+C$或$-\arccos x+C$
<br/><br/>

6. $\int\cos xdx=\sin x+C$
<br/><br/>

7. $\int\sin xdx=-\cos x+C$
<br/><br/>

8. $\int\frac{dx}{\cos^2x}=\tan x+C$
<br/><br/>

9. $\int\frac{dx}{\sin^2x}=-\cot x+C$
<br/><br/>

10. $\int\sec x\tan xdx=\sec x+C$
<br/><br/>

11. $\int\csc x\cot xdx=-\csc x+C$
<br/><br/>

12. $\int e^xdx=e^x+C$
<br/><br/>

13. $a^xdx=\frac{a^x}{\ln a}+C$
<br/><br/>

**三、不定积分的性质**

**性质1:**

设函数$f(x)$和$g(x)$的原函数存在，则:

$\int[f(x)+g(x)]dx=\int f(x)dx+\int g(x)dx$.

**推论:** 若$f(x)=\sum_{i=1}^nk_if_i(x)$,则:

$\int f(x)dx=\sum_{i=1}^nk_i\int f_i(x)dx$

**性质2:**

设函数$f(x)$的原函数存在，k为非零常数，则:

$\int kf(x)dx=k\int f(x)dx$

注意: 检验积分结果是否正确，只要对结果求导，看它的导数是否等于被积函数，相等时结果是正确的，否则结果是错误的

## 4-2: 换元积分法

把复合函数的微分法反过来用于求不定积分，利用中间变量的代换，得到符合函数的积分法，称为换元积分法

### 第一类换元法

**定理1:**

设$f(x)$具有原函数，$u=\phi(x)$可导，则有换元公式:

$\int f[\phi(x)]\phi'(x)dx=[\int f(u)du](u=\phi(x))$

一般地，对于积分$f(ax+b)dx(a\neq0),$总可做变换$u=ax+b$,把它化为:

$\int f(ax+b)dx=\int\frac1af(ax+b)d(ax+b)=\frac1a[\int f(u)du]_{u=ax+b}$

<br/><br/>

一般地，对于$\sin^{2k+1}x\cos^nx$或$\sin^nx\cos^{2k+1}x$(其中k $\in$ N)型函数的积分，总可依次作变换$u=\cos x$或$u=\sin x$,从而求得结果
<br/><br/>

一般地，对于$\sin^{2k}x\cos^{2l}x(k,l\in N)$型函数，总可利用降幂升角三角恒等式$\sin^2x=\frac12(1-\cos2x),\cos^2x=\frac12(1+\cos2x)$化成$\cos2x$的多项式，然后求解.
<br/><br/>

一般地，对于$\tan^nx\sec^{2k}x$或$\tan^{2k-1}x\sec^nx(n,k\in N_+)$型函数的积分，可依次做变换$u=\tan x$或$u=\sec x$,求得结果

总结: 第一类换元法是$u=\phi(x)$

而接下来的第二类换元法是$x=\psi(t)$

### 第二类换元法

适当地选择变量代换$x=\psi(t)$,将积分$\int f(x)dx$化为积分$\int f[\psi(t)]\psi'(t)dt$

该公式成立**需要一定条件**。首先，等式右边的不定积分要存在，即$f[\psi(t)]\psi'(t)$有原函数；

其次，$\int f[\psi(t)]\psi'(t)dt$求出后必须用$x=\psi(t)$的反函数$t=\psi^{-1}(x)$代换回去，为了保证这反函数存在而且是可导的，假定直接函数$x=\psi(t)$在t的某一个区间(这区间和所考虑的x的积分区间相对应)上是单调的，可导的，并且$\psi'(t)\neq0$

一般的第二类换元法是利用三角代换或双曲正余弦代换

**定理2:**

设$x=\psi(t)$是单调的可导函数，并且$\psi'(t)\neq0$.又设$f[\psi(t)]\psi'(t)$具有原函数，则有换元公式:

$\int f(x)dx=[\int f[\psi(t)]\psi'(t)dt]_{t=\psi^{-1}(x)}$

其中$\psi^{-1}(x)$是$x=\psi(t)$的反函数

说明:

（1）. 被积函数含有$\sqrt{x^2+a^2}$或$\sqrt{x^2-a^2}$时，除采用三角代换外，还可利用公式$ch^2t - sh^2t=1$.采用双曲代换$x=asht$或$x=acht$消去根式，所得结果一致

（2）. 如果被积函数含有$\sqrt{x^2+a^2}$,可以作代换$x=a\tan t$化去根式；

（3）. 为了去除被积函数分母中的变量因子x时，可以采用**倒代换**的方法即用原自变量的倒数进行替换

**补充基本积分表(重要):**

(14). $\int shxdx=chx+C$
<br/><br/>

(15). $\int chxdx=shx+C$
<br/><br/>

(16). $\int\tan xdx=-\ln|\cos x|+C$
<br/><br/>

(17). $\int\cot xdx=\ln|\sin x|+C$
<br/><br/>

(18). $\int\sec xdx=\ln|\sec x+\tan x|+C$
<br/><br/>

(19). $\int\csc xdx=\ln|\csc x-\cot x|+C$
<br/><br/>

(20). $\int\frac{dx}{a^2+x^2}=\frac1a\arctan\frac xa+C$
<br/><br/>

(21). $\int\frac{dx}{x^2-a^2}=\frac{1}{2a}\ln|\frac{x-a}{x+a}|+C$
<br/><br/>

(22). $\int\frac1{\sqrt{a^2-x^2}}=\arcsin\frac xa+C$
<br/><br/>

(23). $\int\frac{dx}{\sqrt{x^2+a^2}}=\ln(x+\sqrt{x^2+a^2})+C$
<br/><br/>

(24). $\int\frac{dx}{\sqrt{x^2-a^2}}=\ln|x+\sqrt{x^2-a^2}|+C$
<br/><br/>

## 4-3: 分部积分法

前面的换元积分法是基于复合函数求导法则；而现在利用两个函数乘积的求导法则，来推得另一个求积分的基本方法--分部积分法

由$(uv)'=u'v+uv'$,移项得:

$uv'=(uv)'-u'v$

两边求不定积分得: $\int uv'dx=uv-\int u'vdx$

该公式称为分部积分公式，也可将该公式写成如下形式:

$\int udv=uv-\int vdu$

应用分部积分法时，选取u和dv一般要考虑下面两点:

1. v要容易求得；

2. $\int vdu$要比$\int udv$容易积出

而**保留u**的优先顺序应当尽量遵循以下函数的顺序:(重要)

反函数->对数函数->幂函数->指数函数->三角函数

简称为 **反对幂指三**

其中反函数包括反三角函数和反双曲函数等

## 4-4: 有理函数的积分

两个多项式的商$\frac{P(x)}{Q(x)}$称为有理函数，又称有理分式。当分子多项式$P(x)$的次数小于分母多项式$Q(x)$的次数时，称这有理函数为真分式，否则称为假分式。

对于真分式$\frac{P(x)}{Q(x)}$,如果分母可分解为几个多项式的乘积:

$Q(x)=Q_1(x)\cdot Q_2(x)\cdots Q(n)$

且$Q_1(x)\cdot Q_2(x)\cdots Q(n)$没有公因式，那么它可拆分成几个真分式之和:

$\frac{P(x)}{Q(x)}=\frac{P_1(x)}{Q_1(x)}+\frac{P_2(x)}{Q_2(x)}+\cdots+\frac{P_n(x)}{Q_n(x)}$

最后，有理函数的分解式中只出现 1.多项式，2.$\frac{P_1(x)}{(x-a)^k}$、3.$\frac{P_2(x)}{(x^2+px+q)^l}$等三类函数(**注意:** 这里$p^2-4q< 0,P_1(x)$为小于$k$次的多项式，$P_2(x)$为小于$2l$次的多项式)时，多项式的积分容易求得

**二、可化为有理函数的积分举例**

（1）.通常求含$\sin^2x,\cos^x$以及$\sin x\cos x$的有理式的积分时，用代换$u=\tan x$往往更方便；并且可以用$u=\tan \frac x2$即**万能公式**来代替所有其他三角函数

万能公式如下:

$\LARGE{\sin x=\frac{2\tan\frac x2}{1+\tan^2\frac x2}}$

$\LARGE{\cos x=\frac{1-\tan^2\frac x2}{1+\tan^2\frac x2}}$

（2）.如果被积函数中含有简单根式$\sqrt[n]{ax+b}$或$\sqrt[n]{\frac{ax+b}{cx+d}}$,可以令这个简单公式为u。由于这样的变换具有反函数，且反函数是u的有理函数，因此原积分可以化为有理函数的积分

## 4-5: 积分表的使用

把常见的积分公式汇集成表，这种表叫做**积分表**.积分表是按照被积函数的类型来排列的。求积分时，可根据被积函数的类型直接地经过简单的变形后，在表内查得所需的结果

积分表的整理在下面的链接中:




