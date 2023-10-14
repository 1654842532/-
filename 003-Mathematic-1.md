---
title: 003-Mathematic-1
date: 2023-02-26 20:53:41
tags:
categories: [Mathematic]
toc: true
---


本次笔记相关教材为同济第七版高等数学以及习题全解指南两本书

# 003-Mathematic-高数笔记

## 1-5:极限的运算法则

两个无穷小的和是无穷小
有限个无穷小的和也是无穷小
有界函数与无穷小的乘积是无穷小
**有限个**无穷小的乘积是无穷小

容易忘记的运算法则:
如果 $\lim{f_{(x)}}$存在，而n为正整数，则：$\lim{[f_{(x)}]^{n} = [\lim{f_{(x)}}]^{n}}$

数列的极限运算法则同上，因为数列是一种特殊的函数

注：在求解极限时，首先要观察分母为不为0，若为0，则要用**无穷小无穷大的倒数关系**进行反求解。

线性组合的极限等于极限的线性组合

无穷小无穷大的倒数关系：无穷大的倒数为无穷小，**非0无穷小**的倒数为无穷大

(重要)当 $a_{0},b_{0}$ 都不为0且m和n为非负整数时：

$$ \lim_{x \to \infty} { { a_{0}x^{m}+a_{1}x^{m-1}+ \cdots + a_{m } } \over {b_{0}x^{n}+b_{1}x^{n-1}+ \cdots + b_{n} } } = \begin{cases} {0},& \text{当n>m} \\ {\frac{a_{0} } { b_{0} } } ,& \text{当n=m} \\ \infty ,& \text{当n<m} \end{cases} $$

## 1-6:极限存在准则 两个重要极限

**准则 Ⅰ**(数列夹逼准则): 如果数列 $x_{n},y_{n}及z_{n}满足下列条件:$
(1).从某项起,就 $\exists n_{0} \in N_{+}$, 当n> $n_{0}$ 时，有:
$$ y_{n} \leq x_{n} \leq z_{n} $$
(2). $\lim_{n \to \infty} {y_{n}} = a, \lim_{n \to \infty} {z_{n}} = a$

那么数列 $x_{n}$ 的极限存在， 且 $\lim_{n \to \infty} x_{n} = a$

**准则 $Ⅰ^{\prime}$**(函数夹逼准则):
如果：
(1). 当 x$\in \mathring{U}(x_0,r)$时，存在:
$g_{(x)} \leq f_{(x)} \leq h_{(x)}$

(2). $\lim_{x \to x_{0}} g_{(x)}=A, \lim_{x \to x_{0}}h_{(x)}=A$

那么$\lim_{x \to x_{0}}f_{(x)}$存在，且等于A

准则Ⅰ及准则 $Ⅰ^{\prime}$称为夹逼准则

夹逼准则能够证明第一个重要极限,即:
**$$ \lim_{x \to 0} \frac{sin(x)}{x}=1 $$**

证明：
首先$\frac{sin(x)}{x}$对于一切$x\neq0$都有定义
然后做出一个在第一象限的四分之一单位圆并作标记如图:
[![ppPj9A0.jpg](https://s1.ax1x.com/2023/03/01/ppPj9A0.jpg)](https://imgse.com/i/ppPj9A0)

首先补充说明:

$\overset{\LARGE{\frown}}{弧l}=\alpha × radius$

$S_{扇形}=\frac 12×\overset{\LARGE{\frown}}{弧l}× radius$

可以看出: $BC=\sin(x),AD=\tan(x),\overset{\LARGE{\frown}}{AB}=x$

$\because S_{\Delta AOB}<S_{扇形AOB}<S_{\Delta AOD}$

$\therefore $根据面积公式然后化简可以得出下面这个不等式:

$\sin x < x < \tan x$

不等式各边都除以 $\sin x$得到:

$1 < \frac{x}{\sin x} < \frac 1{\cos x}$

或者 $\cos x< \frac{\sin x}x<1$

$\because$ 当x用-x代替时

$\cos x$与$\frac{\sin x}{x}$ 都不变

所以上面的不等式对于开区间 $(-\frac \pi2,0)$ 内的一切x也是成立的

当$0<|x|<\frac \pi2$时:

$0<|\cos x-1|=1-\cos x=2\sin ^{2}\frac x2 < 2(\frac x2)^2=\frac {x^2}2$

即: $0<1-\cos x<\frac {x^2}2$

而 $\frac {x^2}2 \to 0(x \to 0)$.由准则Ⅰ有:

$\lim_{x \to 0}(1-\cos x) =0$

$\therefore \lim_{x \to 0}\cos x = 1$

根据准则 $Ⅰ^{\prime}$得:

**$\lim_{x \to 0}\frac {\sin x}x=1$**

证毕

说明:只要做题时看到这两个特点:
1.sin后面的式子和分母的式子相同(可以把x换成$\phi_{(x)}$)

2.不但$\phi_{(x)}$可以替代x，且$\phi_{(x)}也趋向于0$
则极限为1

**准则Ⅱ: 单调有界数列必有极限**

利用准则Ⅱ可以推导出第二个重要极限: **$\lim_{x \to \infty}(1+\frac 1x)^x=e$**

在证明之前，要先引入牛顿的二项式定理:

$(a+b)^n=C_{n}^0a^n+C_{n}^1a^{n-1}b+C_{n}^2a^{n-1}b^2+ \cdots +C_{n}^nb^n$

其中 $T_{r+1}=C_{n}^ra^{n-r}b^r$为二项式展开式的通项公式

$T_{r+1}$是展开式中的第k+1项,不是第k项

二项式系数和为$2^n$,即$C_{n}^0+C_n^1+C_n^2+ \cdots +C_n^n = 2^n$

证：
先考虑x取正整数n的情况，设$X_n=(1+\frac 1n)^n$,根据牛顿的二项式定理:

$(1+\frac 1n)^n=C_n^0+C_n^1\frac 1n+C_n^2\frac 1{n^2}+\cdots +C_n^{n-1}\frac 1{n^{(n-1)}}+C_n^n(\frac 1n)^n$

$=1+\frac n1 \frac 1n+\frac {n(n-1)}{2!}\frac 1{n^2}+ \frac {n(n-1)(n-2)}{3!}\frac 1{n^3}+\cdots +\frac {n(n-1)\cdots 2}{(n-1)!}\frac 1{n^{n-1}}+\frac {n!}{n!}\frac 1{n^n}$

$= 1+1+\frac 1{2!}(1-\frac 1n)+\frac 1{3!}(1-\frac 1n)(1-\frac 2n)+\cdots +\frac 1{(n-1)!}(1-\frac 1n)(1-\frac 2n)\cdots (1-\frac {n-2}{n})$

$+ \frac 1{n!}(1-\frac 1n)(1-\frac 2n)\cdots (1-\frac{n-1}n)$

类似地:

$X_{n+1}=(1+\frac 1{n+1})^{n+1}$

$=1+1+\frac 1{2!}(1-\frac 1{n+1})+\frac 1{3!}(1-\frac 1{n+1})(1-\frac 2{n+1})+\cdots$

$+\frac 1{n!}(1-\frac 1{n+1})(1-\frac 2{n+1})\cdots (1-\frac {n-1}{n+1})+\frac 1{(n+1)!}(1-\frac 1{n+1})(1- \frac 2{n+1})\cdots$

$(1-\frac n{n+1})$

比较$X_n$,$X_{n+1}$的展开式，可以看到除了前两项外,$X_n$的每一项都小于$X_{n+1}$的对应项，并且 $X_{n+1}$还多了最后的一项，其值大于0，

$\therefore X_n<X_{n+1}$

说明数列{$X_n$}是单调增加的

这个数列同时还是有界的。因为如果$X_n$的展开式中各项括号内的数用较大的数1代替，得:

$X_n \leq 1+(1+\frac 1{2!}+\frac 1{3!}+\cdots +\frac 1{n!})\leq 1+(1+\frac 12+\frac 1{2^2}+\cdots +\frac 1{2^{n-1}})$

$=1+\frac {1-\frac 1{2^n}}{1-\frac 12}=3-\frac 1{2^{n-1}}<3$

说明 $X_n$是有界的，根据准则Ⅱ推出这个数列${X_n}$得极限存在

通常用字母e来表示它，即:

$\lim_{n \to \infty}(1+\frac 1n)^n=e$

数列证完了，就要从数列推导至函数：

采用的方法依然是夹逼准则

设 n $\leq x <n+1$

则: $(1+\frac 1{n+1})^n<(1+\frac 1x)^x<(1+\frac 1n)^{n+1}$

分别求两边极限然后利用夹逼法则可以得出极限为e

然后令 x=-(t+1) 则 x->-$\infty$时，t->+$\infty$

再求出极限为e(x->-$\infty$)

$\therefore \lim_{x \to \infty}(1+\frac 1x)^x=e$

e=2.718281828459045


然后代换得

$$ \lim_{z \to 0}(1+z)^{\frac 1z}=e $$

证毕

准则$Ⅱ^{\prime}$: 设函数fx在点$x_0$的某个左邻域内单调且有界，则fx在$x_0$的左极限$f_{x_0^-}$必定存在

**柯西(Cauchy)极限存在准则:**
数列{$X_n$}收敛的充分必要条件是:对于任意给定的正数$\epsilon$,存在正整数N，使得当m>N,n>N时，有|$X_n-X_m$|<$\epsilon$

小知识点:
设x为任一实数，不超过x的最大整数称为x的整数部分，记作[x]
可以得出一个推论: **[x]>x-1**, 因为[x]再怎么不超过x，x的整数部分与x的距离都不可能超过1

## 1-7：无穷小的比较

反映了不同的无穷小趋于0的“快慢”程度
高阶无穷小: $B = o(\alpha)$
低阶无穷小
同阶无穷小
k阶无穷小
等价无穷小: $B$~$\alpha$

**一个重要的等价无穷小:**
当$x \to 0$, $\sqrt[n]{1+x}-1$~$\frac 1nx$
或者写成: $(1+x)^a-1$~$ax(x \to 0)$

证明用到了高阶多项式因式分解公式:
$a^n-b^n=(a-b)(a^{n-1}b^0+a^{n-2}b^1+a^{n-3}b2+\cdots +a^0b^{n-1})$
以及分子有理化

**定理2(重要)**:
设$\alpha$~$\~\alpha$, $B$~$\~B$,且$\lim \frac {\~B}{\~\alpha}$存在，则:

$\lim \frac B\alpha =\lim \frac {\~B}{\~\alpha}$

***当x$\to$0时，常见且非常重要的一些等价无穷小:***

$\sin x$~ $x$~$\tan x$~$\arcsin x$~$\ln (x+1)$~$e^x-1$

$1-\cos x$~$\frac 12x^2$

$(1+x)^a-1$~$ax$

**(重要)** 同一变化过程中，$\alpha,B$为无穷小，根据等价无穷小，可得:

(1).和差取大规则:若$B=o(\alpha)$,则$\alpha \pm B$~$\alpha$

(2).和差替代规则: 若$\alpha$~$\~\alpha$, $B$~$\~B$,**且$B与\alpha$不等价**,则 $\alpha -B$~$\~\alpha -\~B$
注意：$\alpha$~$B$时此结论不一定成立，要考虑别的办法

(3).若$\alpha$~$B$,且$\phi_{(x)}$存在或有界，则$\lim \alpha \phi_{(x)}=\lim B\phi_{(x)}$

## 1-8:函数的连续点与间断点

设函数fx在点$x_0$的某一邻域内有定义，如果:

$\lim_{x \to x_0} f_{(x)}=f_{(x_0)}$

那么就称函数fx在点$x_0$连续

左连续与右连续类似于连续的定义

如果说让你证明函数在某个区间连续,则就是证明

$\Delta y \to 0(\Delta x \to 0)$

方法可以利用夹逼准则

补充知识:
1.积化和差公式
$\sin \alpha \cos B=\frac 12[\sin (\alpha +B)+\sin (\alpha-B)]$
$\cos \alpha \sin B=\frac 12[\sin (\alpha+B)-\sin(\alpha-B)]$
$\cos\alpha\cos B=\frac 12[\cos(\alpha+B)+\cos(\alpha-B)]$
$\sin \alpha\sin B=\frac 12[\cos(\alpha-B)-\cos(\alpha+B)]$

2.和差化积公式
$\sin\alpha+\sin B=2\sin\frac {\alpha+B}{2}\cos\frac {\alpha-B}2$
$\sin\alpha-\sin B=2\cos\frac {\alpha+B}2\sin\frac {\alpha-B}2$
$\cos\alpha+\cos B=2\cos\frac {\alpha+B}2\cos\frac {\alpha-B}2$
$\cos\alpha-\cos B=2\sin\frac {\alpha+B}2\sin\frac {\alpha-B}2$

设函数fx在点$x_0$的某去心邻域内有定义。在此前提下，如果函数fx有下列三种情况任何一种之一:

1.在x=$x_0$没有定义

2.虽然在x=$x_0$有定义，但是$\lim_{x \to x_0}f_{(x)}$不存在

3.虽然在x=$x_0$有定义且$\lim_{x \to x_0}f_{(x)}$存在，但是$\lim_{x \to x_0}f_{(x)}\neq f_{(x_0)}$

则点$x_0$为fx的间断点

几种常见间断点:
1.无穷间断点(第二类)
2.振荡间断点(第二类)
3.可去间断点(第一类)
4.跳跃间断点(第一类)

## 1-9连续函数的运算与初等函数的连续性

设函数$f_{(x)}$与$g_{(x)}$在点$x_0$连续，则它们的和、积、差、商($g_{(x_0)}\neq 0$)都在点 $x_0$连续

如果函数fx在区间I上单调增加(或单调减少)且连续，那么它的反函数$f^{-1}$也在对应的区间上单调增加(或单调减少)(证明采用定义法)

$\lim_{x \to x_0}f_{g_{(x)}}=\lim_{u \to u_0}f_{u}=f_{u_0}$

**(重要)** 基本初等函数在它们的定义域内都是连续的
一切初等函数在其定义区间内都是连续的

## 1-10闭区间上连续函数的性质

**有界性与最大最小值定理**:
在闭区间上连续的函数在该区间上有界且一定能取得它的最大值和最小值

**(重要)零点定理**:
设函数$f_{(x)}$在闭区间[a,b]上连续，且$f_{(a)}与f_{(b)}$异号
即$f_{(a)}×f_{(b)}<0,$则在开区间(a,b)内至少有一点$\xi$使$f_{(\xi)}=0$

**介值定理**
设函数$f_{(x)}$在闭区间[a,b]上连续，且在这区间的端点取不同函数值
$f_{(a)}=A, f_{(b)}=B$
则对于A与B之间(不包括A与B)的任意一个数C，在开区间(a,b)内至少有一点$\xi$使得 $f_{(\xi)}=C (a<\xi<b)$

证明采用的是构造函数加零点定理

**一致连续性**:存在着只与$\epsilon$有关，而对区间I上任何点$x_0$都能适用的正数$\delta$,即对任何$x_0 \in I$,只要|x-$x_0$|<$\delta$时，就有|$f_{(x)}-f_{(x_0)}$|<$\epsilon$
如果fx在区间I上能使这种情况发生，就说函数fx在区间I上是一致连续的。

**一致连续性定理**:如果函数$f_{x}$在闭区间[a,b]上连续，那么它在该区间上一致连续














