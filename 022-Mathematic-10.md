---
title: 022-Mathematic-10
date: 2023-03-26 19:02:44
categories: [Mathematic]
tags:
toc: true
---

本次笔记相关教材为同济第七版高等数学上册以及习题全解指南两本书

## 5-1: 定积分的概念与性质

计算曲边梯形的面积: 在区间[a,b]中任意插入若干个分点$a=x_0< x_1< x_2< \cdots< x_{n-1}< x_n=b$,

把[a,b]分成几个小区间$[x_0,x_1],[x_1,x_2],\cdots,[x_{n-1},x_n]$,它们的长度依次为:

$\Delta x_1=x_1-x_0, \Delta x_2=x_2-x_1,\cdots,\Delta x_n=x_n-x_{n-1}$.

经过每一个分点作平行于y轴的直线段，把曲边梯形分成n个窄曲边梯形。在每个小区间$[x_{i-1},x_i]$上任取一点$\xi$,以$[x_{i-1},x_i]$为底，$f(\xi_i)$为高的窄矩形近似替代第i个窄曲边梯形(i=1,2,...,n)，把这样得到的几个窄矩形的面积之和作为所求曲边梯形面积A的近似值，即

$A\approx f(\xi_1)\Delta x_1+f(\xi_2)\Delta x_2+\cdots+f(\xi_n)\Delta x_n=\sum_{i=1}^nf(\xi_i)\Delta x_i$.

为了保证所有小区间的长度都无限缩小，我们要求小区间长度中的最大者趋于零，比如，记$\lambda=max{\Delta x_1,\Delta x_2,\cdots,\Delta x_n}$

则上述条件可表示为$\lambda\to0$.当$\lambda\to0$时(这时分段数n无限增多，即$n\to\infty$),取上述和式的极限，便得到曲边梯形的面积:

$A=\lim_{\lambda=0}\sum_{i=1}^nf(\xi_i)\Delta x_i$

**定义:** 设函数$f(x)$在[a,b]上有界，在[a,b]中任意插入若干个分点

$a=x_0< x_1< x_2< \cdots< x_{n-1}< x_n=b$,把区间[a,b]分成n个小区间$[x_0,x_1],[x_1,x_2],\cdots,[x_{n-1},x_n]$，各个小区间的长度依次为:

$\Delta x_1=x_1-x_0, \Delta x_2=x_2-x_1,\cdots,\Delta x_n=x_n-x_{n-1}$.

在每个小区间$[x_{i-1},x_i]$上任取一点$\xi_i(x_{i-1}< \xi_i< x_i)$,作函数值$f(\xi_i)$与小区间长度$\Delta x_i$的乘积$f(\xi_i)\Delta x_i(i=1,2,\cdots,n)$,并做出和:

$S=\sum_{i=1}^nf(\xi_i)\Delta x_i$.

记$\lambda=max\{\Delta x_1,\Delta x_2,\cdots,\Delta x_n\}$,

如果当$\lambda\to0$时，这和的极限总存在，且与闭区间[a,b]的分法及点$\xi_i$的取法无关，那么称这个极限I为函数$f(x)$在区间[a,b]上的定积分(简称积分)，记作

$\int_a^b\sum_{i=1}nf(\xi_i)\Delta x_i$,

其中$f(x)$叫做被积函数，$f(x)dx$叫做被积表达式，$x$叫做积分变量，a叫做积分下限，b叫做积分上限，[a,b]叫做积分区间

**注意:**

当和式$\sum_{i=1}^nf(\xi_i)\Delta x_i$的极限存在时，其极限I仅与被积函数$f(x)$和积分区间[a,b]有关。如果既不改变被积函数f,也不改变积分区间[a,b],而只把积分变量x改写成其他字母，例如t或者u,那么，这时和的极限I不变，也就是定积分的值不变，即:

$\int_a^bf(x)dx=\int_a^bf(t)dt=\int_a^bf(u)du$.

这就是说，**定积分的值只与被积函数及积分区间有关，而与积分变量的记法无关**。

如果$f(x)$在[a,b]上的定积分存在，那么就说$f(x)$在[a,b]上可积。

$f(x)$在[a,b]上满足怎样的条件，$f(x)$在[a,b]上一定可积？这里不做深入探讨，但给出以下两个充分条件:

**定理1:** 设$f(x)$在[a,b]上连续，则$f(x)$在[a,b]上可积

**定理2:** 设$f(x)$在[a,b]上有界，且只有有限个间断点，则$f(x)$在[a,b]上可积

**定积分的几何意义:**

当在[a,b]上$f(x)\leq0$时，由曲线$y=f(x)$、两条直线$x=a,x=b$与x轴所围成的曲边梯形位于x轴的下方，定积分$\int_a^bf(x)dx$表示上述曲边梯形面积的负值；在[a,b]上$f(x)$既取得正值又取得负值时，函数$f(x)$的图形某些部分在x轴的上方，而其他部分在x轴下方，此时定积分$\int^b_af(x)dx$表示x轴上方图形面积减去x轴下方图形面积所得之差

### 定积分的性质:

补充:

（1）、当b=a时，$\int_a^bf(x)dx=0;$

（2）、当a>b时，$\int_a^bf(x)dx=-\int_b^af(x)dx$

即交换定积分的上下限时，定积分的绝对值不变而符号相反

**性质1:** 设$\alpha$与$\beta$均为常数，则:

$\int_a^b[\alpha f(x)+\beta g(x)]=\alpha\int_a^bf(x)dx+\beta\int_a^bg(x)dx$

性质1对于任意有限个函数的线性组合也是成立的

**性质2:** 设$a< c< b$,则:

$\int_a^bf(x)dx=\int_a^cf(x)dx+\int_c^bf(x)dx$

这个性质表明定积分对于积分区间具有可加性。

且补充规定: 不论a,b,c的相对位置如何，总有等式成立:

$\int_a^bf(x)dx=\int_a^cf(x)dx+\int_c^bf(x)dx$ 

例如: 当$a< b< c$时，由于$\int_a^cf(x)dx=\int_a^bf(x)dx+\int_b^cf(x)dx$

于是得: $\int_a^bf(x)dx=\int_a^cf(x)dx-\int_b^cf(x)dx$

$=\int_a^cf(x)dx+\int_c^bf(x)dx$

**性质3：**

如果在区间[a,b]上$f(x)=1$,那么:

$\int_a^b1dx=\int_a^bdx=b-a$

**性质4:**

如果在区间[a,b]上$f(x)\geq0,$那么$\int_a^bf(x)dx\geq0(a< b)$

**推论1:**

如果在区间[a,b]上$f(x)\leq g(x)$,那么:

$\int_a^bf(x)dx\leq\int_a^bg(x)dx (a< b)$

**推论2：**

$|\int_a^bf(x)dx|\leq\int_a^b|f(x)|dx$

利用几何意义理解便可

**性质5:**

设M及m分别是函数$f(x)$在区间[a,b]上得最大值及最小值，则:

$m(b-a)\leq\int_a^bf(x)dx\leq M(b-a)\:\:(a< b)$

这个性质说明，由被积函数在积分区间上的最大值及最小值，可以估计积分值的大致范围

**性质6:(定积分中值定理)**

如果函数$f(x)$在积分区间[a,b]上连续，那么在[a,b]上至少存在一个点$\xi$,使下式成立:

$\int_a^bf(x)dx=f(\xi)(b-a)\:\:(a\leq\xi< b)$

这个公式叫做积分中值公式

证明方法1: 闭区间上连续函数的最大最小值定理 + 闭区间上连续函数的介值定理。

证明方法2: 牛顿-莱布尼茨公式 + 拉格朗日中值定理

**积分中值公式的几何解释:**

在区间[a,b]上至少存在一点$\xi$,使得以区间[a,b]为底边、以曲线$y=f(x)$为曲边的曲边梯形的面积等于同一底边而高为$f(\xi)$的一个矩形的面积

按积分中值公式所得: $f(\xi)=\frac1{b-a}\int_a^bf(x)dx$

称为函数$f(x)$在区间[a,b]上的平均值

## 5-2：微积分基本公式

设函数$f(x)$在区间[a,b]上连续，并且设x为[a,b]上一点。我们来考察$f(x)$在部分区间[a,x]上的定积分$\int_a^xf(x)dx$:

首先，由于$f(x)$在[a,x]上仍旧连续，因此这个定积分存在。这里，x既表示定积分的上限，又表示积分变量。因为定积分与积分变量的记法无关，所以，为了明确起见，可以把积分变量改用其他符号，例如用t表示，则上面的定积分可以写成:

$\int_a^xf(t)dt$

如果上限x在区间[a,b]上任意变动，那么对于每一个取定的x值，定积分有一个对应值，所以它在[a,b]上定义了一个函数，记作$\Phi(x)$:

$\Phi(x)=\int_a^xf(t)dt\:\:(a\leq x\leq b)$

这个函数$\Phi(x)$具有下面定理1所指出的重要性质.

**定理1:**

如果函数$f(x)$在区间[a,b]上连续，那么积分上限的函数

$\Phi(x)=\int_a^xf(t)dt$在[a,b]上可导，并且它的导数:

$\Phi'(x)=\frac d{dx}\:\int_a^xf(t)dt=f(x)\:\:(a\leq x\leq b)$

**证:**

若$x\in(a,b),$设x获得增量$\Delta x$，其绝对值足够地小,使得$x+\Delta x\in(a,b)$,则$\Phi(x)$在$x+\Delta x$处的函数值为:$\Phi(x+\Delta x)=\int_a^{x+\Delta}f(t)dt$.

由此得函数的增量$\Delta\Phi=\Phi(x+\Delta x)-\Phi(x)$

$=\int_a^{x+\Delta x}f(t)dt-\int_a^xf(t)dt$

$=\int_a^xf(t)dt+\int_x^{x+\Delta x}f(t)dt-\int_a^xf(t)dt$

$=\int_x^{x+\Delta x}f(t)dt$

再应用积分中值定理，即有等式$\Delta\Phi=f(\xi)\Delta x$

这里，$\xi$在$x,x+\Delta x$之间。把上式两端各除以$\Delta x$,得函数增量与自变量增量的比值$\frac{\Delta\Phi}{\Delta x}=f(\xi)$.

由于假设$f(x)$在[a,b]上连续，而$\Delta x\to0$时，$\xi\to x$,因此$\lim_{\Delta x\to0}f(\xi)=f(x).$于是，令$\Delta x\to0$对上式两端取极限时，左端的极限也应该存在且等于$f(x)$.

这就是说，函数$\Phi(x)$的导数存在，并且$\Phi'(x)=f(x)$.

若$x=a$,取$\Delta x> 0$,则同理可证$\Phi_+'(a)=f(a)$;

若$x=b$,取$\Delta x< 0$,则同理可证$\Phi_-'(b)=f(b)$

**证毕**

该定理指出了一个重要结论:

连续函数$f(x)$取变上限$x$的定积分然后求导，其结果还原为$f(x)$本身

**定理2:**

如果函数$f(x)$在区间[a,b]上连续，那么函数: $\Phi(x)=\int_a^xf(t)dt$ 就是$f(x)$在[a,b]上的一个原函数

### 牛顿--莱布尼茨公式(重要)

**定理3:(微积分基本定理)**

如果函数$F(x)$是连续函数$f(x)$在区间[a,b]上的一个原函数，那么$\int_a^bf(x)dx=F(b)-F(a)$

**证:**

已知函数$F(x)$是连续函数$f(x)$的一个原函数，又根据定理2知道，积分上限的函数$\Phi(x)=\int_a^xf(t)dt$ 也是$f(x)$的一个原函数。

于是这两个原函数之差$F(x)-\Phi(x)$在[a,b]上必定是某一个常数C，即:

$F(x)-\Phi(x)=C(a\leq x\leq b)$

在上式中令$x=a$,得$F(a)-\Phi(a)=C$,又由$\Phi(x)$的定义式可得: $\Phi(a)=0$.

因此，$C=F(a)$.

以$F(a)$代入$F(x)-\Phi(x)=C$中的C，以$\int_a^xf(t)dt$代入其中的$\Phi(x)$,可得:

$\int_a^xf(t)dt=F(x)-F(a)$.

在上式中令x=b,就得到所要证明的公式

**证毕**

该公式对$a> b$的情形同样成立。

为了方便起见，以后把$F(b)-F(a)$记成$[F(x)]_a^b$,于是原式又可写成:

$\int_a^bf(x)dx=[F(x)]_a^b$

该公式叫做牛顿(Newton)-莱布尼茨(Leibniz)公式，也叫做微积分基本公式。

它表明: 一个连续函数在区间[a,b]上的定积分等于它的任意一个原函数在区间[a,b]上的增量。

说明：

一、连续函数的原函数一定存在；

二、其他变限积分求导：

①、$\frac1{dx}\int_x^bf(t)dt=-f(x)$;
<br/><br/>

②、$\frac{d}{dx}\int_a^{\phi(x)}f(t)dt=f[\phi(x)]\phi'(x)$
<br/><br/>

③、$\frac{d}{dx}\int^{\phi(x)}_{\psi(x)}f(t)dt$
<br/><br/>

$=\frac{d}{dx}[\int_{\psi(x)}^af(t)dt+\int_a^{\phi(x)}f(t)dt]$
<br/><br/>

$=f[\phi(x)]\phi'(x)-f[\psi(x)]\psi'(x)$

## 5-3: 定积分的换元法和分部积分法

### 定理1:(定积分的换元法)

假设函数$f(x)$在区间[a,b]上连续，函数$x=\phi(t)$满足条件:

(1). $\phi(\alpha)=a,\phi(\beta)=b$;

(2). $\phi(t)$在$[\alpha,\beta]$(或$[\beta,\alpha]$)上具有连续函数，且其值域$R_\phi=[a,b]$,

则有$\int_a^bf(x)dx=\int_\alpha^\beta f[\phi(t)]\phi'(t)dt$.

该公式叫做定积分的换元公式

说明: 1. 当$\beta< \alpha$时，即区间换为$[\beta,\alpha]$时，定理1仍成立

2.必须注意换元必换限，原函数中的变量不必代回

3.换元公式也可反过来使用，即

$\int_\alpha^\beta f[\phi(t)]\phi'(t)dt=\int_a^bf(x)dx$(令$x=\phi(t)$)

或者配元: $\int_\alpha^\beta f[\phi(t)]\phi'(t)dt=\int_\alpha^\beta f[\phi(t)]d(\phi(t))$

并且**配元是不换限的**,只有换元才换限

4.在积分区间关于原点对称时，可以考查被积函数的**奇偶性**:

如果是奇函数，则原定积分为0;如果是偶函数，则原定积分只要考虑其中一边的积分区间的结果，然后乘以2就行了。这就是通常所说的 **"偶倍奇零"**

5.$\int_0^{\frac\pi2}f(\sin x)dx=\int_0^{\frac\pi2}f(\cos x)dx$

证明方法是换元法+诱导公式

$\int_0^\pi xf(\sin x)dx=\frac\pi2\int_0^\pi f(\sin x)dx$

证明方法是换元法

6.设$f(x)$是连续的周期函数，则有公式如下:

(1). $\int_a^{a+T}f(x)dx=\int_0^Tf(x)dx$

**证:**
记$\Phi(a)=\int_a^{a+T}f(x)dx$,则:

$\Phi'(a)=[\int_0^{a+T}f(x)dx-\int_0^af(x)dx]'$

$=f(a+T)-f(a)=0$

因此$\Phi(a)$与a无关，因此$\Phi(a)=\Phi(0)$,即:

$\int_a^{a+T}f(x)dx=\int_0^Tf(x)dx$

**证毕**

(2). $\int_a^{a+nT}f(x)dx=n\int_0^Tf(x)$

**证:**

$\int_a^{a+nT}f(x)dx=\sum_{k=0}^{n-1}\int_{a+KT}^{a+KT+T}f(x)dx$

由（1）得:$\int_{a+KT}^{a+KT+T}f(x)dx=\int_0^Tf(x)dx$,

$\therefore \int_a^{a+nT}f(x)dx=n\int_a^Tf(x)dx$

**证毕**

### 定积分的分部积分法

依据不定积分的分部积分法，可得:

$\int_a^bu(x)v'(x)dx=[\int u(x)v'(x)dx]_a^b$

$=[u(x)v(x)-\int v(x)u'(x)dx]_a^b$

$=[u(x)v(x)]_a^b-\int_a^bv(x)u'(x)dx$

简记作: $\int_a^b uv'dx=[uv]_a^b-\int_a^bvu'dx$

或者$\int_a^budv=[uv]_a^b-\int_a^bvdu$

该公式叫做定积分的分部积分公式

利用分部积分法可以推出一个实用的定积分公式，叫**点火公式**:

$I_n=\int_0^{\frac\pi2}\sin^nxdx=\int_0^{\frac\pi2}\cos^nxdx$

$=\begin{cases}\frac{n-1}n\cdot\frac{n-3}{n-2}\cdot\cdots\cdot\frac34\cdot\frac12\cdot\frac\pi2,&\text{n为正偶数}\\\\\frac{n-1}n\cdot\frac{n-3}{n-2}\cdot\cdots\cdot\frac45\cdot\frac23,& n为大于1的正奇数 \end{cases}$

**证:**

$I_n=-\int_0^{\frac\pi2}\sin^{n-1}xd(\cos x)$

$=[-\cos x\sin^{n-1}x]_0^{\frac\pi2}+(n-1)\int_0^{\frac\pi2}\sin^nxdx$

上面的式子中第一项等于零；将第二项里的$\cos^2x$写成$1-\sin^2x$,并把积分分成两个，得:

$I_n=(n-1)\int_0^{\frac\pi2}\sin^{n-2}xdx-(n-1)\int_0^{\frac\pi2}\sin^nxdx$

$=(n-1)I_{n-2}-(n-1)I_n$

由此得: $I_n=\frac{n-1}nI_{n-2}$ (用分部积分法求出递推公式)

这个等式叫做积分$I_n$关于下标的递推公式

令$n=n-2$得:

$I_{n-2}=\frac{n-3}{n-2}I_{n-4}$

同样地依次进行下去，直到$I_n$的下标递减到0或1为止，于是:

$I_{2m}=\frac{2m-1}{2m}\cdot\frac{2m-3}{2m-2}\cdot\cdots\cdot\frac56\cdot\frac34\cdot\frac12\cdot I_0$,

$I_{2m+1}=\frac{2m}{2m+1}\cdot\frac{2m-2}{2m-1}\cdot\cdots\cdot\frac67\cdot\frac45\cdot\frac23\cdot I_1,(m=1,2,\cdots)$

而$I_0=\int_0^{\frac\pi2}dx=\frac\pi2,I_1=\int_0^{\frac\pi2}\sin xdx=1$

因此: 

$I_{2m}=\frac{2m-1}{2m}\cdot\frac{2m-3}{2m-2}\cdot\cdots\cdot\frac56\cdot\frac34\cdot\frac12\cdot\frac\pi2$

$I_{2m+1}=\frac{2m}{2m+1}\cdot\frac{2m-2}{2m-1}\cdot\cdots\cdot\frac67\cdot\frac45\cdot\frac23,m=(1,2,\cdots)$

**证毕**

## 5-4:反常积分

### 无穷限的反常积分

设函数$f(x)$在区间$[a,+\infty)$上连续，任取$t> a$,作定积分$\int_a^tf(x)dx$, 再求极限:

$\lim_{t\to+\infty}\int_a^tf(x)dx$

这个对变上限定积分的算式称为函数$f(x)$在无穷区间$[a,+\infty]$上的反常积分，记为$\int_a^{+\infty}$,即:

$\int_a^{+\infty}=\lim_{t\to+\infty}\int_a^tf(x)dx$

**定义 1:**

（1）、设函数$f(x)$在区间$[a,+\infty)$上连续，如果极限$\lim_{t\to+\infty}\int_a^tf(x)dx$存在，那么称反常积分$\int_a^{+\infty}f(x)dx$收敛，并称此极限为该反常积分的值；

如果该极限不存在，那么称反常积分$\int_a^{+\infty}f(x)dx$发散
<br/>

（2）、设函数$f(x)$在区间$(-\infty,b]$上连续，如果极限$\lim_{t\to-\infty}\int_t^bf(x)dx$存在，那么称反常积分$\int_{-\infty}bf(x)dx$收敛，并称此极限为该反常积分的值；

如果该极限不存在，那么称反常积分$\int_{-\infty}^bf(x)dx$发散
<br/>

（3）、设函数$f(x)$在区间$(-\infty,+\infty)$上连续，如果反常积分$\int_{-\infty}^0f(x)dx$与反常积分$\int_0^{+\infty}f(x)dx$**均收敛**,那么称反常积分$\int{-\infty}{+\infty}f(x)dx$收敛，

并称反常积分$\int_{-\infty}^0f(x)dx$的值与反常积分$\int_0^{+\infty}f(x)dx$的值之和为反常积分$\int{-\infty}{+\infty}f(x)dx$的值，否则就称反常积分$\int{-\infty}{+\infty}f(x)dx$发散
<br/>

上述反常积分统称为无穷限的反常积分

### 牛顿-莱布尼茨公式推测反常积分的收敛性

利用牛顿-莱布尼茨公式可以推测反常积分是收敛的还是发散的:

设$F(x)$为$f(x)$在$[a,+\infty]$上的原函数，则:

$\int_a^{+\infty}f(x)dx=\lim_{x\to+\infty}F(x)\:-F(a)$

若$\lim_{x\to+\infty}F(x)$存在，则收敛;反之发散

若记该极限为$F(+\infty)$,则:

$\int_a^{+\infty}f(x)dx=[F(x)]_a^{+\infty}$

类似地可以用于$\int_{-\infty}^bf(x)dx$

注意: 若在$(-\infty,+\infty)$内$F'(x)=f(x),$则当$F(-\infty),F(+\infty)$都存在时，

$\int_{-\infty}^{+\infty}f(x)dx=[F(x)]_{-\infty}^{+\infty}$

当$F(-\infty)$与$F(+\infty)$有一个不存在时，反常积分$\int_{-\infty}^{+\infty}f(x)dx$发散。

**说明:**

（1）、有时通过换元，反常积分和常义积分可以相互转化，从而简便运算；

（2）、当一题中含有两类反常积分时，应当划分积分区间，然后分别讨论每一个区间上的反常积分；

（3）、有时需要考虑主值意义下的反常积分，其定义为:

$v.p.\int_{-\infty}^{+\infty}f(x)dx=\lim_{a\to+\infty}\int_{-a}^af(x)dx$

注意: 主值意义下的反常积分存在不等于一般意义下的常义积分收敛

### 无界函数的反常积分

如果函数$f(x)$在点a的任一邻域内都无界，那么点a称为函数$f(x)$的瑕点(也称为无界间断点)。无界函数的反常积分又称为瑕积分。

设函数$f(x)$在区间$(a,b]$上连续，点a为$f(x)$的瑕点。任取$t> a$,作定积分$\int_t^bf(x)dx$,再求极限$\lim_{t\to a^+}\int_t^bf(x)dx$,

这个对变下限的定积分求极限的算式称为函数$f(x)$在区间$[a,b]$上的反常积分，仍然记为$\int_a^bf(x)dx$,即:

$\int_a^bf(x)dx=\lim_{t\to a^+}\int_t^bf(x)dx$

**定义2:**

（1）、设函数$f(x)$在区间$(a,b]$上连续，点a为$f(x)$的瑕点，如果极限$\lim_{t\to a^+}\int_t^bf(x)dx$存在，那么称反常积分$\int_a^b$收敛，并称此极限为该反常积分的值；如果极限不存在，那么反常积分发散

类似地可以定义在[a,b)上的$\int_a^bf(x)dx$(b为f(x)的瑕点)

以及在[a,c]及(c,b]上的$\int_a^bf(x)dx$(c为f(x)的瑕点)

<br/>

无界函数的反常积分，也可借助于牛顿-莱布尼茨公式

设$x=a$为$f(x)$的瑕点:

$\therefore\int_a^bf(x)dx=F(b)-\lim_{x\to a^+}F(x)$

$=F(b)-F(a^+)$

同样，对于$x=b$和$x=c$为瑕点的情况也是一个道理

### 补充两个重要的反常积分:

（1）、反常积分$\int_a^{+\infty}\frac{dx}{x^p}\:\:(a>0)$

当$p>1$时收敛；

当$p\leq 1$时发散

（2）、反常积分$\int_a^b\frac{dx}{(x-a)^q}$

当$0< q < 1$时收敛

当$q\geq1$时发散

## 5-5：反常积分的审敛法 $\:\Gamma$函数

### 无穷限反常积分的审敛法

**定理1:**

设函数$f(x)$在区间$[a,+\infty)$上连续，且$f(x)\geq 0$.

若函数$F(x)=\int_a^xf(t)dt$在$[a,+\infty)$上 **有上界** ，则反常积分$\int_a^{+\infty}f(x)dx$收敛。

解释: 事实上，因为$f(x)\geq0,F(x)$在$[a,+\infty)$上单调增加，又$F(x)$在$[a,+\infty)$上有上界，故$F(x)$在$[a,+\infty)$上是单调有界的函数。

按照$[a,+\infty)$上的单调有界函数$F(x)$必有极限$\lim_{x\to+\infty}F(x)$的准则，就可知道极限$\lim_{x\to+\infty}\int_a^xf(t)dt$存在，即反常积分$\int_a^{+\infty}f(x)dx$收敛

<br/>

**定理2(比较审敛原理):**

设函数$f(x),g(x)$在区间$[a,+\infty)$上连续。

如果$0\leq f(x)\leq g(x)\:\:(a\leq x< +\infty)$,并且$\int_a^{+\infty}g(x)dx$收敛，那么$\int_a^{+\infty}f(x)dx$也收敛；

如果$0\leq g(x)\leq f(x)\:\:(a\leq x< +\infty)$,并且$\int_a^{+\infty}g(x)dx$发散，那么$\int_a^{+\infty}f(x)dx$也发散

**证:**

设$a< t< +\infty$,由$0\leq f(x)\leq g(x)$及$\int_a^{+\infty}g(x)dx$收敛，得:

$\int_a^tf(x)dx\leq\int_a^tg(x)dx\leq\int_a^{+\infty}g(x)dx$

这表明作为积分上限t的函数:

$F(t)=\int_a^tf(x)dx$

在$[a,+\infty)$上有上界。由定理1知反常积分$\int_a^{+\infty}f(x)dx$收敛

如果$0\leq g(x)\leq f(x)$,且$\int_a^{+\infty}g(x)dx$发散，那么$\int_a^{+\infty}f(x)dx$必定发散。因为如果$\int_a^{+\infty}f(x)dx$收敛，由定理的第一部分即知$\int_a^{+\infty}g(x)dx$也收敛，这与假设相矛盾

**证毕**

**定理3(比较审敛法1,利用了$\int_a^{+\infty}\frac{dx}{x^p}$当p取不同区间的收敛情况):**

设函数$f(x)$在区间$[a,+\infty)(a> 0)$上连续，且$f(x)\geq 0$.

如果存在常数$M> 0$及$p>1,$使得$f(x)\leq\frac M{x^p}(a\leq x< +\infty),$那么反常积分$\int_a^{+\infty}f(x)dx$收敛；

如果存在常数$N> 0$,使得$f(x)\geq \frac Nx(a\leq x< +\infty),$那么反常积分$\int_a^{+\infty}f(x)dx$发散

**定理4(极限审敛法1):**

设函数$f(x)$在区间$[a,+\infty)$上连续，且$f(x)\geq0$.

如果存在常数$p> 1$,使得$\lim_{x\to+\infty}x^pf(x)=c< +\infty$,

那么，反常积分$\int_a^{+\infty}f(x)dx$收敛;

如果$\lim_{x\to+\infty}xf(x)d> 0$(或$\lim_{x\to+\infty}xf(x)=+\infty$),那么反常积分$\int_a^{+\infty}f(x)dx$发散

**定理5:**

设函数$f(x)$在区间$[a,+\infty)$上连续，如果反常积分$\int_a^{+\infty}|f(x)|dx$收敛，

那么反常积分$\int_a^{+\infty}f(x)dx$也收敛。

通常称满足定理5条件的反常积分$\int_a^{+\infty}f(x)dx$**绝对收敛**

于是，定理5可以简单地表达为:

绝对收敛的反常积分$\int_a^{+\infty}f(x)dx$必定收敛

### 无界函数的反常积分的审敛法

**定理6(比较审敛法2):**

设函数$f(x)$在区间$(a,b]$上连续，且$f(x)\geq0$

$x=a$为$f(x)$的瑕点。

如果存在常数$M> 0$以及$q< 1$,使得:

$f(x)\leq \frac M{(x-a)^q}\:\:(a< x\leq b)$,

那么反常积分$\int_a^bf(x)dx$收敛

如果存在常数$N> 0$,使得:

$f(x)\geq \frac{N}{x-a}(a<x \leq b)$,

那么反常积分$\int_a^bf(x)dx$发散

**定理7(极限审敛法2):**

设函数$f(x)$在区间$(a,b]$上连续，且$f(x)\geq0$

$x=a$为$f(x)$的瑕点

如果存在常数$0< q< 1$,使得

$\lim_{x\to a^+}(x-a)^qf(x)$ 存在，

那么反常积分$\int_a^bf(x)dx$收敛；

如果$\lim_{x\to a^+}(x-a)f(x)=d> 0$(或$\lim_{x\to a^+}(x-a)f(x)=+\infty$)

那么反常积分$\int_a^bf(x)dx$发散

对于无界函数的反常积分，当被积函数在所讨论的区间上可取正值也可取负值时，有与定理5相类似的结论，在此不再详述

### $\Gamma$函数

$\Gamma$函数的定义是:

$\Gamma(s)=\int_0^{+\infty}e^{-x}x^{s-1}dx\:\:(x> 0)$

根据前面的知识可以推出: $\Gamma$函数对$s> 0$均收敛

$\Gamma$函数的几个重要性质:

（1）、递推公式: $\Gamma(s+1)=s\Gamma(s)\:\:(s>0)$

证明方法: 应用分部积分法

一般地，对于任何正整数n,有$\Gamma(n+1)=n!$.

所以，我们可以把$\Gamma$函数看成是阶乘的推广

（2）、当$s\to0^+$时，$\Gamma(s)\to+\infty$

**证:**

$\because\Gamma(s)=\frac{\Gamma(s+1)}s,\:\:\Gamma(1)=1$

$\therefore s\to0^+$时，$\Gamma(x)\to+\infty$

（3）、$\Gamma(s)\Gamma(1-s)=\frac{\pi}{\sin \pi s}(0< s< 1)$

这个公式称为**余元公式**,证明不要求掌握

当$s=\frac12$时，由余元公式可得: $\Gamma(\frac12)=\sqrt{\pi}$

（4）、在$\Gamma(s)=\int_0^{+\infty}e^{-x}x^{s-1}dx$中

作代换$x=u^2$,有:

$$ \Gamma(s)=2\int_0^{+\infty}e^{-u^2}u^{2s-1}du.\tag{式1}$$

再令$2s-1=t$或$s=\frac{1+t}2$,即有:

$\int_0^{+\infty}e^{-u^2}u^tdu=\frac12\Gamma(\frac{1+t}2)\:\:(t> -1)$

上式左端是实际应用中常见的积分，它的值可以通过上式用$\Gamma$函数计算出来

在(式1)中，令$s=\frac12,$得:

$2\int_0^{+\infty}e^{-u^2}du=\Gamma(\frac12)=\sqrt{\pi}$

从而$\int_0^{+\infty}e^{-u^2}du=\frac{\sqrt{\pi}}2$

上式左端的积分是在概率论中常用的积分

