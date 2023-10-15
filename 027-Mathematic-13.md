---
title: 027-Mathematic-13
date: 2023-10-13 08:14:56
tags:
---

# 第七章习题总结

题1: 一个半球体形状的雪堆,其体积融化率与半球面面积A成正比,比例系数 k > 0. 假设在融化过程中雪堆始终保持半球体形态,已知半径为 $r_{0}$ 的雪堆在开始融化的3小时内融化了其体积的 $\frac78$ , 问雪堆全部融化需要多少时间?

<details>

<summary>解析:</summary>

设雪堆在时刻t的体积为 $V=\frac23\pi r^{3}$ , 侧面积 $S=2\pi r^{2}$ .

由题设可知:

$\frac{dV}{dt}=2\pi r^{2}\frac{dr}{dt}=-kS=-2\pi kr^{2}$ .

$\therefore \frac{dr}{dt}=-k$ .

两边积分得: $r=-kt +C$

由 $r|_{t=0}=r_{0}$ 得: 

$C=r_{0}, r=r_{0} - kt$

由 $V|_{t=3}=\frac18V|_{t=0}$

即: $\frac23\pi (r_{0}-3k)^{3}=\frac18\cdot\frac23\pi r_{0}^3$

得 $k=\frac16 r_{0}$

从而: $r=r_{0}-\frac16 r_{0}t$

令 $r=0$ 得 t=6

$\therefore$ 全部融化需要6小时

</details>

题2: 求微分方程的通解: $(1+2e^{\frac xy})dx+2e^{\frac xy}(1-\frac xy)dy=0$

<details>

<summary>解析:</summary>

令 $u=\frac xy$ , $\therefore x=uy, \frac{dx}{dy}=u+y\frac{du}{dy}$

代入原方程得:

$u+y\frac{du}{dy}=\frac{2e^{u}(u-1)}{1+2e^{u}}$

$\therefore y\frac{du}{dy}=-\frac{u+2e^{u}}{1+2e^{u}}$

$\therefore \frac{(1+2e^{u})du}{u+2e^{u}}=-\frac{dy}{y}$

两边积分得:

$\ln|u+2e^{u}|+\ln y=\ln C_{1}$

即 $y(u+2e^{u})=\pm C_{1}$

将 $u=\frac xy$ 代入上式得通解:

$x+2ye^{\frac xy}=C$

思路: 同样是齐次方程,有时也要考虑到 $\frac xy$ 的应用

</details>

题3: 求下面的齐次方程满足所给初值条件的特解:

$(y^{2}-3x^{2})dy+2xydx=0, y|_{x=0}=1$

<details>

<summary>解析:</summary>

原方程可写成: 

$1-3\frac{x^{2}}{y^{2}}+2\frac xy\frac{dx}{dy}=0$

令 $u=\frac xy$

$\therefore x=yu, \frac{dx}{dy}=u+y\frac{du}{dy}$

$\therefore$ 原方程化为:

$1-3u^{2}+2u(u+y\frac{du}{dy})=0$

分离变量得:

$\frac{2u}{u^{2}-1}du=\frac{dy}{y}$

两边积分得:

$\ln|u^{2}-1|=\ln|y|+\ln C_{1}$

$\therefore u^{2}-1=Cy$

代入 $u=\frac xy$得:

$x^{2}-y^2=Cy^{3}$

$\because x=0,y=0$

得 $C=-1$

$\therefore$ 特解为:

$y^{3}=y^{2}-x^{2}$

思路: 同样是齐次方程,有时也要考虑到 $\frac xy$ 的应用

</details>

题4: 求下面的齐次方程满足所给初值条件的特解:

$(x^{2}+2xy-y^{2})dx+(y^{2}+2xy-x^{2})dy=0, y|_{x=1}=1$

<details>

<summary>解析:</summary>

$\frac{dy}{dx}=\frac{y^{2}-2xy-x^{2}}{y^{2}+2xy-x^{2}}=\frac{(\frac yx)^{2}-2\frac yx-1}{(\frac yx)^{2}+2\frac yx-1}$

令$\frac yx=u, \therefore y=xu, \frac{dy}{dx}=u+x\frac{du}{dx}$

$\therefore u+x\frac{du}{dx}=\frac{u^{2}-2u-1}{u^{2}+2u-1}$

$\therefore x\frac{du}{dx}=\frac{u^{2}-2u-1-u^{3}-2u^{2}+u}{u^{2}+2u-1}$

$\therefore -\frac{u^{2}+2u-1}{u^{3}+u^{2}+u+1}du=\frac{dx}{x}$

两边积分得:

$\int\frac{1-2u-u^{2}}{u^{3}+u^{2}+u+1}du$

$=\int\frac{1-2u-u^{2}}{(u+1)(u^{2}+1)}du$

$=\int(\frac{1}{u+1}-\frac{2u}{u^{2}+1})du$

$=\ln\frac{|u+1|}{u^{2}+1}$

$\therefore \ln\frac{|u+1|}{u^{2}+1}=\ln|x|+\ln C$

$\therefore \frac{u+1}{u^{2}+1}=Cx$

代入 $u=\frac yx$ 得:

$\frac{y+x}{y^{2}+x^{2}}=C$

代入初值得: C=1

$\therefore \frac{y+x}{y^{2}+x^{2}}=1$

思路: 回忆一下解多项式积分时候的待定系数法

</details>

题5: 验证型如 $yf(xy)dx+xg(xy)dy=0$ 的微分方程可经变量代换 $v=xy$化为可分离变量的方程,并求其通解

<details>

<summary>解析:</summary>

由 $v=xy$ , 即 $y=\frac vx, dy=\frac{xdv-vdx}{x^{2}}$

首先将原方程两端同乘x得:

$xyf(xy)dx + x^{2}g(xy)dy=0$

并将 $v=xy, dy=\frac{xdv-vdx}{x^{2}}$ 代入上式得:

$vf(v)dx+g(v)(xdv-vdx)=0$

可分离变量得:

$\frac{g(v)dv}{v[f(v)-g(v)]}+\frac{dx}{x}=0$

两边积分得:

$\int\frac{g(v)dv}{v[f(v)-g(v)]}+\ln|x|=C$

代入 $v=xy$ 后, 便是原方程的通解

思路： 首先要想到原方程同乘x,然后接下来转化慢慢分离变量即可.

</details>

题6: 求微分方程的通解:

$y^{3}y''-1=0$

<details>

<summary>解析:</summary>

令 $y'=p, y''=p\frac{dp}{dy}$

代入原方程得:

$y^{3}\cdot p\frac{dp}{dy}-1=0$

$\therefore pdp=\frac{dy}{y^{3}}$

两边积分得:

$p^{2}=-\frac{1}{y^2}+C_{1}$

$\therefore y'=\pm\sqrt{C_{1}-\frac{1}{y^{2}}}=\pm\frac{1}{|y|}\sqrt{C_{1}y^{2}-1}$ (积分转化的关键)

分离变量得:

$\frac{|y|dy}{\sqrt{C_{1}y^{2}-1}}=\pm\int dx$

由于 $|y|=y\cdot sgn(y)$

其中 $sgn(y)=\begin{cases} 1, & \text{y ≥ 0 } \\ \\ -1, & \text{y < 0} \end{cases}$

应用到两端积分得:

$sgn(y)\int\frac{ydy}{\sqrt{C_{1}y^{2}-1}}=\pm\int dx$

$\therefore sgn(y)\int\frac{ydy}{\sqrt{C_{1}y^{2}-1}}=\pm C_{1}x+C_{2}$

两边平方得:

$C_{1}y^{2}-1=(C_{1}x+C_{2})^{2}$

思路: 抽出 $\frac 1y$ 对于接下来积分很重要,不然很难解开; 然后还有sgn函数的应用

</details>

题7: 求微分方程的通解:

$y''=\frac{1}{\sqrt{y}}$

<details>

<summary>解析:</summary>

令 $y'=p, y''=p\frac{dp}{dy}$

$\therefore p\frac{dp}{dy}=\frac {1}{\sqrt{y}}$

分离变量并两边积分得:

$p^{2}=4\sqrt{y}+C_{1}$

$\therefore \frac{dy}{dx}=\pm\sqrt{4\sqrt{y}+C_{1}}$

分离变量求积分, 先求左边:

$\int\frac{dy}{\sqrt{4\sqrt{y}+C_{1}}}$

$=\int\frac{2\sqrt{y}d(\sqrt{y})}{\sqrt{4\sqrt{y}+C_{1}}}$

令 $u=\sqrt{y}$

$\therefore$ 原式

$=2\int\frac{ud(u)}{\sqrt{4u+C_{1}}}$

$=\frac 12\int\frac{4u+C_{1}-C_{1}}{\sqrt{4u+C_{1}}}dx$

$=\frac 12 \int\sqrt{4u+C_{1}}d(u)-\frac 12\int\frac{1}{\sqrt{4u+C_{1}}}d(u)$

接下来代入积分公式即可

思路: 难点在于 $\sqrt{\sqrt{y}}$ 如何处理

</details>

题8: 求下面的微分方程满足所给初值条件的特解:

$y''+(y')^{2}=1, y|_{x=0}=0, y'|_{x=0}=0$

<details>

<summary>解析: </summary>

令 $y'=p, y''=p\frac{dp}{dy}$

代入原方程得:

$p\frac{dp}{dy}+p^{2}=1$

分离变量得:

$\frac{pdp}{1-p^{2}}=dy$

两边积分得:

$-\frac 12\ln(1-p^{2})=y+ C_{1}$

而由 $y=0,y'=0$ 得: $C_{1}=0$

$\therefore p=\pm\sqrt{1-e^{-2y}}$

再分离变量得:

$\frac{dy}{\sqrt{1-e^{-2y}}}=\pm x$

两边积分,求左边积分:

$\int\frac{dy}{\sqrt{1-e^{-2y}}}$

$=\int\frac{d(e^{y})}{\sqrt{e^{2y}-1}}$

$=\ln(e^{y}+\sqrt{e^{2y}-1})$

$\therefore \ln(e^{y}+\sqrt{e^{2y}-1})=\pm x + C_{2}$

由 y=0, x=0 得: $C_{2}=0$

$\therefore$ 特解为:

$e^{y} = \frac{e^{x}+e^{-x}}{2}$

</details>

题9: 已知 $y=1,y=x,y=x^{2}$ 是某二阶非齐次线性微分方程得三个解,则该方程的通解为:

<details>

<summary>解析:</summary>

由叠加原理知 $x-1$ 与 $x^{2}-1$ 是非齐次方程对应的齐次方程的解, 且它们是线性无关的, 于是根据线性方程通解结构得: 

$y=C_{1}(x-1)+C_{2}(x^{2}-1) +1$

</details>

题10: 设非齐次线性微分方程 $y'+P(x)y=Q(x)$ 有两个不同的解: $y_{1}(x), y_{2}(x)$ , C为任意常数,则该方程的通解是()

A. $C[y_{1}(x)-y_{2}(x)]$

B. $y_{1}(x)+ C[y_{1}(x)-y_{2}(x)]$

C. $C[y_{1}(x)+y_{2}(x)]$

D. $y_{1}(x)+ C[y_{1}(x)+y_{2}(x)]$

<details>

<summary>解析:</summary>

$y_{1}(x)-y_{2}(x)$ 是对应的齐次方程 $y'+P(x)y=0$ 的非零解。

从而由线性微分方程解的性质定理知 $C[y_{1}(x)-y_{2}(x)]$ 是齐次方程的通解,再由非齐次线性方程解的结构定理知:

$y_{1}(x)+ C[y_{1}(x)-y_{2}(x)]$ 是原方程的解

</details>

题11: 具有特解 $y_{1}=e^{-x}, y_{2}=2xe^{-x}, y_{3}=3e^{x}$ 的三阶常系数齐次线性微分方程是()

A. $y'''-y''-y'+y=0$

B. $y'''+y''-y'-y=0$

C. $y'''-6y''+11y'-6y=0$

D. $y'''-2y''-y'+2y=0$

<details>

<summary>解析:</summary>

由题意知: $r=-1,-1,1$ 为所求齐次线性微分方程对应的特征方程的3个根, 而 $(r+1)^{2}(r-1)=r^{3}+r^{2}-r-1$

</details>

题12: 求微分方程的通解:

$y''+2y'+5y=\sin 2x$

<details>

<summary>解析:</summary>

先求齐次方程:

$\because r^{2}+2r+5=0$

解得: $r=\frac{-2\pm \sqrt{-16}}{2} = -1\pm2i$

$\therefore Y=e^{-x}(C_{1}\cos 2x+C_{2}\sin 2x)$

再看 $\sin 2x, \lambda=0,\omega=2$

$\because \lambda \pm\omega i$ 不是特征方程的根

$\therefore k=0$

$\therefore y^{*}=A\cos 2x+B\sin 2x$

代入原方程得:

$(A+4B)\cos 2x+(B-4A)\sin 2x=\sin 2x$

比较系数得:

$\begin{cases} A+4B=0 & \\ \\ B-4A=1 \end{cases}$

得: $A=-\frac {4}{17}, B=\frac {1}{17}$

$\therefore y=Y+y^{*}$

</details>

题13: 求微分方程的通解:

$y'''+y''-2y'=x(e^{x}+4)$

<details>

<summary>解析: </summary>

先解齐次方程:

$r^{3}+r^{2}-2r=0$

得: $r_{1}=0, r_{2}=1, r_{3}=-2$

$\therefore Y=C_{1}+C_{2}e^{x}+C_{3}e^{-2x}$

然后将原方程右端进行分解:

对于方程 $y'''+y''-2y'=xe^{x}$

$\because f_{1}(x)=xe^{x}$ , 其中 $\lambda =1$ 是特征方程中的一个单根.

故令 $y_{1}^{*}=x(A_{1}x+B_{1})e^{x}$

代入上式并消去 $e^{x}$ 得:

$6A_{1}x+8A_{1}+3B_{1}=x$ , 比较系数得:

$\begin{cases} 6A_{1}=1 & \\ \\ 8A_{1}+3B_{1}=0 \end{cases}$

得 $y_{1}^{*}=(\frac 16 x^{2}-\frac 49x)e^{x}$

对于方程 $y'''+y''-2y'=4x$ 

$\because f_{2}(x)=4x,$ 其中 $\lambda=0$ 是特征方程的一个单根

故令 $y_{2}^{*}=x(A_{2}x+B_{2})$

代入方程得: 

$-4A_{2}x+2A_{2}-2B_{2}=4x$

待定系数法解得: $A_{2}=-1, B_{2}=-1$

$\therefore y_{2}^{*}=-x^{2}-x$

根据线性方程解的叠加原理知:

$y^{*} = y_{1}^{*}+ y_{2}^{*}$ 是原方程特解

$\therefore y=Y+y^{*}$

</details>

题14: 求微分方程的通解:

$y'+x=\sqrt{x^{2}+y}$

<details>

<summary>解析: </summary>

令 $\sqrt{x^{2}+y}=u$

$\therefore y=u^{2}-x, y'=2uu'-2x$

$\therefore 2uu'-2x+x=u$

$\therefore\frac{du}{dx}-\frac 12(\frac xu) = \frac {1}{2}$

再令 $\frac {u}{x}=v, \frac{du}{dx}=v+x\frac{dv}{dx}$

原方程化为:

$v+x\frac{dv}{dx}-\frac{1}{2v}=\frac 12$

分离变量得:

$\frac{vdv}{2v^{2}-v-1}=-\frac{1}{2}\frac{dx}{x}$

两边积分得:

$\frac 13[\ln|v-1|+\frac 12\ln|2v-1|]=-\frac 12\ln|x| +C_{1}$

即:

$(v-1)^{2}(2v-1)x^{3}=C_{2}$

代入 $v=\frac uv$ 得:

$2u^{3}-3xu^{2}+x^{3}=C_{2}$

再代入 $v=\frac{u}{x}$ 得原方程通解:

$2(x^{2}+y)^{\frac 32}=x^{3}+\frac 23xy+C(C=\frac 12C_{2})$

</details>


