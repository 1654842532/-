---
title: 012-Mathematic-3
date: 2023-03-08 14:13:26
tags:
toc: true
categories: [Mathematic]
---

本次笔记相关教材为同济第七版高等数学以及习题全解指南两本书

## 2-1:导数概念

设函数 $y=f_{(x)}$ 在点$x_0$的某个邻域内有定义，当自变量$x$在$x_0$处取得增量$\Delta x$(点$x_0+\Delta x$仍在该邻域内)时，相应地，因变量y取得增量$\Delta y=f_{(x_0+\Delta x)}-f_{(x_0)}$.
如果$\Delta y$与$\Delta x$的比值(当$\Delta x\to0$时)的极限存在，那么称函数$y=f_{(x)}$在点$x_0$处可导
并称这个极限为函数$y=f_{(x)}$在点$x_0$处的导数,记为$f_{(x_0)}'$,即:

$f'_{(x_0)}=\lim_{\Delta x\to0}\frac{\Delta y}{\Delta x}=\lim_{\Delta x\to0}\frac{f_{(x_0+\Delta x)}-f_{(x_0)}}{\Delta x}$

也可记作 $y'|_{x=x_0},\frac {dy}{dx}|_{x=0}$ 或 $\frac {d(f_{x})}{dx}|_{x=x_0}$

也可记作 $\lim_{h\to0}\frac{f_{(x_0+h)}-f_{(x_0)}}{h}$

注意: $\lim_{\Delta x\to0}\frac{\Delta y}{\Delta x}$存在一定说明什么? 说明$\Delta y$也是$\Delta x \to0$的无穷小，并且与$\Delta x$同阶或者高阶
所以这句话也包含了$\Delta x\to0,\Delta y\to0$,即**连续的定义**
所以: 可导一定连续
但是从$\Delta x\to0,\Delta y\to0$无法推出$\lim_{\Delta x\to0}\frac {\Delta y}{\Delta x}$存在
所以:连续不一定可导

总结: **可导一定连续，连续不一定可导**

若函数在开区间I内每点都可导，就称函数在I内可导

左导数和右导数: $f'_{-(x_0)}=\lim_{h\to0^-}\frac {f_{(x_0+h)}-f_{(x_0)}}h$
$f'_{+(x_0)}=\lim_{h\to0^+}\frac {f_{(x_0+h)}-f_{(x_0)}}h$

左导数和右导数统称为单侧导数
如果函数$f_{(x)}$在开区间(a,b)内可导,且$f'_{+(a)}$和$f'_{-(b)}$都存在，那么就说$f_{(x)}$在闭区间[a,b]上可导

切线与法线的斜率乘积为 -1

判断可导性的途径:
1. 不连续一定不可导；
2. 直接用导函数的定义；
3. 看左右导数是否存在，并且相等

## 2-2: 函数的求导法则

**定理1**: 如果函数 $u=u_{(x)}$及$v=v_{(x)}$都在点x具有导数，那么它们的和、差、积、商(除分母为0的点外)都在点x具有导数，且:

$(1). [u_{(x)}\pm v_{(x)}]'=u_{(x)}'\pm v'_{(x)};$

$(2). [u_{(x)}v_{(x)}]'=u'_{(x)}v_{(x)}+u_{(x)}v'_{(x)}$

$(3). [\frac{u_{(x)}}{v_{(x)}}]'=\frac{u'_{(x)}v_{(x)}-u_{(x)}v'_{(x)}}{v^2_{(x)}} (v_{(x)}\neq0)$

**推论**: $(uvw)'=u'vw+uv'w+uvw'$

**定理2**: 如果函数$x=f_{(y)}$在区间$I_y$内单调、可导,且$f'_{(y)}\neq0$,那么它的反函数$y=f^{-1}_{(x)}$在区间$I_x=\{x|x=f_{(y)},y\in I_y\}$内也可导,且:

$[f^{-1}_{(x)}]'=\frac 1{f'_{(y)}}$ 或 $\frac {dy}{dx}=\frac 1{\frac{dx}{dy}}$

即: 反函数的导数等于直接函数导数的倒数

补充三角函数公式:

$\arccos x=\frac \pi2-\arcsin x$
arccot $x=\frac \pi2-\arctan x$

**定理3**: 如果$u=g_{(x)}$在点x可导，而$y=f_{(u)}$在点$u=g_{(x)}$可导,那么复合函数 $y=f_{g_{(x)}}$在点x可导，且其导函数为:

$\frac {dy}{dx}=f'_{u}·g'_{x}$ 或 $\frac{dy}{dx}=\frac{dy}{du}·\frac{du}{dx}$

**推广**: 此定理可以推广到多层中间变量的情况。关键是搞清复合函数的结构，由外向内逐层求导

**(重要)** 一些基本的公式加导数公式(需要牢牢记住)

首先说明: 最基本的公式为:
1. $(C)'=0$
2. $(\sin x)'=\cos x$
3. $(\ln x)'=\frac 1x$

上面三个公式用定义法来证明，然后其他导数公式用求导法推出即可

1. $(C)'=0$

2. $(x^\mu)'=\mu·x^{\mu-1}$

3. $(\sin x)'=\cos x$

4. $(\cos x)'=-\sin x$

5. $(\tan x)'=\sec^2x$

6. $(\sec x)'=\sec x\tan x$

7. $(\csc x)'=-\csc x\cot x$

8. $(\cot x)'=-\csc^2x$

9. $(a^x)'=a^x·\ln a(a>0且a\neq1)$

10. $(e^x)'=e^x$

11. $(\log_ax)'=\frac1{x·\ln a}(a>0且a\neq1)$

12. $(\ln x)'=\frac 1x$

13. $\arcsin x=\frac \pi2-\arccos x$

14. $\arctan x=\frac \pi2-arccot x$

15. $(\arcsin x)'=\frac 1{\sqrt{1-x^2}}$

16. $(\arccos x)'=-\frac 1{\sqrt{1-x^2}}$

17. $(\arctan x)'=\frac 1{1+x^2}$

18. $(arccotx)'=-\frac 1{1+x^2}$

19. $sh 2x=2sh xch x$

20. $ch 2x=ch^2x+sh^2x$

21. $ch^2x-sh^2x=1$

22. $(sh x)'=ch x$

23. $(ch x)'=sh x$

24. $(th x)'=\frac 1{ch^2x}$

25. arsh $x=\ln(x+\sqrt{1+x^2})$

26. arch $x=\ln(x+\sqrt{x^2-1})$

27. arth $x=\frac 12\ln\frac{1+x}{1-x}$

28. (arsh $x)'=\frac1{\sqrt{1+x^2}}$

29. (arch $x)'=\frac1{\sqrt{x^2-1}}$

30. (arth $x)'=\frac1{1-x^2}$

31. $\sec^2x-\tan^2x=1$

## 2-3: 高阶导数

二阶导数记作: $\frac{d^2y}{dx^2}$ 或 $f''_{(x)}$

$y=f_{(x)}$具有n阶导数，也常说成函数$f_{(x)}$为n阶可导函数.
如果函数$f_{(x)}$在点$x_0$处具有n阶导数，那么$f_{(x)}$在点x的某一邻域内必定具有一切低于n阶的导数
二阶及二阶以上的导数统称为高阶导数

**(重要)** 几个初等函数的n阶导数:

1. $(\sin x)^{(n)}=\sin(x+n·\frac\pi2)$

2. $(\cos x)^{(n)}=\cos(x+n·\frac\pi2)$

3. $[\ln(1+x)]^{(n)}=(-1)^{(n-1)}\frac{(n-1)!}{(1+x)^n}$

4. $[\ln(1-x)]^{(n)}=-\frac{(n-1)!}{(1-x)^n}$

5. $(x^\mu)^{(n)}=\mu(\mu-1)\cdots(\mu-n+1)x^{\mu-n}$

6. $(e^{ax}\sin bx)^{(n)}=(a^2+b^2)^{\frac2n}·e^{ax}·\sin(bx+\phi)$(其中$\phi=\arctan(\frac ba)$)

**莱布尼茨公式(Leibniz)**:

$(u+v)^{(n)}=\sum_{k=0}^{n}C_n^ku^{(n-k)}v^{(k)}$

阶数很高时，莱布尼茨公式往往到了某一项时会变为常数求导，即为0

**一些基本公式**:

1. $C_n^0+C_n^1+\cdots+C_n^n=2^n$

2. $rC_n^r=nC_{n-1}^{r-1}$

3. $C_n^{k-1}+C_n^k=C_{n+1}^k$

4. $C_n^r=C_n^{n-r}$

5. $1^2+2^2+\cdots+n^2=\frac{n\cdot(n+1)\cdot(2n+1)}6$

公式五的证明方法是根据立方差公式

$(a+1)^3-a^3=3a^2+3a+1$ 中的平方项采用累加的方式得出

6. $a^3-b^3=(a-b)(a^2+ab+b^2)$

7. $a^3+b^3=(a+b)(a^2-ab+b^2)$

**方法补充:**

1. 继两边取对数之后，又多了一个非常好的方法，叫两边取导数(**重要**,考研考察两边取导数以及引申的对数求导法的频率非常高)

2. 常常利用导数的递推公式来研究问题，而导数的递推公式则由两边取导数推出

## 2-4: 隐函数及由参数方程所确定的函数的导数 相关变化率

一般地，如果变量x和y满足一个方程$F_{(x,y)}=0$,在一定条件下，当x取某区间内的任一值时，相应地总有满足这方程的唯一的y值存在，那么就说方程$F_{(x,y)}=0$在该区间内确定了一个隐函数

有时需要计算隐函数的导数，因此，方法就是**两边取对数**

说明: 对于幂指函数$y=u^v$，可用**对数求导法**:
对数求导法就是先两边取对数，再两边取导数

$\ln y=v\ln u$

$\therefore\frac1y\cdot y'=v'\ln u+\frac{u'v}u$

$\therefore y'=u^v(v'\ln u+\frac{u'v}u)$

即$y'=u^v\ln u\cdot v'+vu^{v-1}\cdot u'$

注：两边取对数对隐函数求导时，因为y是无法直接求出表达式的，所以在求导函数值时，只能从原方程看出x取某一个值时对应的y的值

一般地，若参数方程 $\begin{cases} x=\phi_{(t)},&\\\\y=\psi_{(t)},&\end{cases}$ 确定y与x之间的函数关系，则称此函数关系所表达的函数为由参数方程所确定的函数，则:

$\frac{dy}{dx}=\frac{\frac{dy}{dt}}{\frac{dx}{dt}}=\frac {\psi'_{(t)}}{\phi'_{(t)}}$

$\frac{d^2y}{dx^2}=\frac d{dt}(\frac{dy}{dx})\frac{dt}{dx}$

$=\frac{d}{dt}(\frac{\psi'_{(t)}}{\phi'_{(t)}})\frac1{\frac{dx}{dt}}$

$=\frac{\psi''_{(t)}\phi'_{(t)}-\psi'_{(t)}\phi''_{(t)}}{\phi'^{3}_{(t)}}$

设$x=x_{(t)}$及$y=y_{(t)}$都是可导函数，而变量x与y之间存在某种关系，从而变化率 $\frac{dx}{dt}$与$\frac{dy}{dt}$也存在一定关系，这两个互相依赖的变化率称为相关变化率

## 2-5: 函数的微分

设函数$y=f_{(x)}$在某区间内有定义，$x_0$及$x_0+\Delta x$在这个区间内，如果函数的增量$\Delta y = f_{(x_0+\Delta x)}-f_{x_0}$可表示为 $\Delta y = A\Delta x+o(\Delta x)$

其中A是不依赖于$\Delta x$的常数，那么称函数$y=f_{(x)}$在点$x_0$是可微的

$A\Delta x$叫做函数$y=f_{(x)}$在点$x_0$相应于自变量增量$\Delta x$的微分，记作 $dy$

**推论**:

如果"$y=f_{(x)}$在某区间内有定义，$x_0$及$x_0+\Delta x$在区间内" 这种描述语句

与"$y=f_{(x)}$ 在点$x_0$的某一邻域内有定义"等价的话

那么 ***可微即可导，二者等价*** ,与连续的关系自然也就是

可导/可微一定连续，连续不一定可导/可微

$A=f'_{(x_0)}$

$\therefore dy=f'_{(x_0)}\Delta x$,称为在某一点$x_0$的微分

我们说，$dy$是$\Delta y$的线性主部

**但是$dy\neq\Delta y, dy$~$\Delta y$**

在$\Delta x$很小时，有近似等式: $\Delta y\approx dy$

函数在任意点x的微分，称为函数的微分，记作

$dy$或$df_{(x)}$

通常把自变量x的增量$\Delta x$称为自变量的微分，记作$dx$,记作

$dx=\Delta x$

$\therefore dy=f'_{(x)}dx$

**微分的四个要点**:

1. 自变量x的微分: $dx=\Delta x$

2. 函数y的微分: $dy=f'_{(x)}dx$ (可导等价于可微)

3. 函数微分与函数增量的关系: $\Delta y\approx dx$
(即函数微分是函数增量的线性主部)

4. $\Delta x$很小时，有近似计算公式: $f_{(x)}\approx f_{(x_0)}+f'_{(x_0)}\Delta x$

微分的几何意义:

对于可微函数$f_{(x)}$而言，当$\Delta y$是曲线$y=f_{(x)}$上的点的纵坐标的增量时，$dy$就是曲线的切线上点的纵坐标的相应增量

当$|\Delta x|$很小时，$|\Delta y-dy|$比$|\Delta x|$小得多。因此可以用切线段来近似代替曲线段

这在数学上称为非线性函数的局部性优化

微分公式就是导数公式的变形公式，所以只要导数公式记熟，微分公式自然也就记熟了

函数和、差、积、商、复合函数，这些的微分法则依然与导数时的情况相同

**微分在近似计算中的运用**:

$f_{(x)}=f_{(x_0)}+f'_{(x_0)}(x-x_0)$ (条件是|$x-x_0$|很小)

当x与0很接近时，又可以得到:

$f_{(x)}=f_{(0)}+f'_{(0)}x$

所以，当$|x|$都是较小的数值时，可以使用以下常见的数学公式:

1. $(1+x)^\alpha - 1 \approx\alpha x$

2. $\sin x\approx x$

3. $\ln(x+1)\approx x$

4. $x\approx\tan x$

5. $1-\cos x\approx\frac12x^2$

6. $e^x-1\approx x$

7. $x\approx nx$

**误差估计:**

如果某个量的精确值为A,它的近似值为$\alpha$,那么$|A-\alpha|$叫做$\alpha$的**绝对误差**

而绝对误差与$|\alpha|$的比值$\frac{|A-\alpha|}{|\alpha|}$叫做$\alpha$的**相对误差**

如果某个量的精确值为A,它的近似值为$\alpha$，又知道它的误差不超过$\delta_A$,即: $|A-\alpha|\leq\delta_A$

那么$\delta_A$叫做测量A的**绝对误差限**

而$\frac{\delta_A}{|\alpha|}$叫做测量A的**相对误差限**

一般地，根据直接测量的x值按公式$y=f_{(x)}$计算y值时，如果已知测量x的绝对误差限是$\delta_x$,即 $|\Delta x|\leq\delta_x$

那么，当$y'\neq0$时，y的绝对误差:

$|\Delta y|\approx|dy|=|y'|\cdot|\Delta x|\leq|y'|\cdot\delta_x$

即y的绝对误差限约为 $\delta_y=|y'|\cdot \delta_x$

y的相对误差限约为 $\frac{\delta_y}{|y|}=|\frac {y'}y|\cdot\delta_x$

以后常把绝对误差限与相对误差限简称为绝对误差与相对误差





