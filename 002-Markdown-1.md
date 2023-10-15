---
title: '002-Markdown-1'
date: 2023-02-28 16:01:08
tags:
categories: [Markdown]
toc: true
---


感谢博主 <a href="https://blog.csdn.net/qq_38253837?type=blog">healer-c</a>提供的<a href="https://blog.csdn.net/qq_38253837/article/details/109923758">文章</a>, 受益匪浅


# 002-Markdown-数学笔记需要用到的语法

## 如何插入公式

1. 行中插入公式:

`$数学公式$`
例如: \$y=ax+b\$
显示: $y=ax+b$

2. 与正文独立插入公式

`$$ 数学公式 $$`
例如: \$\$ y=ax+b \$\$
显示: 

$$ y=ax+b $$

## 常见数学符号和公式

### 1.上下标

显示|代码|描述
-|-|-
$x^{2}$ | \$ x^{2} \$ |上标
$x_{i}$ | \$ x_{i} \$ | 下标

### 2.括号和分隔符
()、[]和|可以直接输入

显示|代码|显示|代码|描述
-|-|-|-|-
$\langle$ | \$ \langle \$ | $\rangle$ | \$ \rangle \$ | 尖括号
$\{$ | \$\\{\$ | $\}$ | \$\\}\$ | 花括号

### 3.分数

* 分数通常使用 **\frac{分子}{分母}**,如:

显示|代码
-|-
$\frac{x^{2}}{y}$|\$\frac{x^{2}}{y}\$

* 分式较为复杂时，可以使用**分子 \over 分母表示**，如：

显示|代码
-|-
$a+b^{2}+c+d+e+f \over g+h+i+j+k+l$  |\$ a+b^{2}+c+d+e+f \over g+h+i+j+k+l \$

所以当分式仅有两个字符时，可以使用 **\frac ab** 来快速生成 $\frac ab$

### 4.开方
使用 `sqrt[根指数，默认为2]{被开方数}`，如：

显示|代码
-|-
$\sqrt{2}$|\$ \sqrt{2} \$
$\sqrt[n]{5}$|\$ \sqrt[n]{5} \$

### 5.向量和箭头

显示|代码|描述
-|-|-
$\vec{x}$|\$ \vec{x} \$|向量x
$\overleftarrow{x}$|\$ \overleftarrow{x} \$|x上方左箭头
$\overrightarrow{x}$|\$ \overrightarrow{x} \$|x上方向右箭头
$\leftarrow$|\$ \leftarrow \$|左箭头
$\rightarrow$|\$ \rightarrow \$|右箭头
$\uparrow$|\$ \uparrow \$|向上的箭头
$\downarrow$|\$ \downarrow \$|向下的箭头
$\Leftarrow$|\$ \Leftarrow \$|
$\Rightarrow$|\$ \Rightarrow \$|
$\Uparrow$|\$ \Uparrow \$|
$\Downarrow$|\$ \Downarrow \$|

### 6.积分

使用`\int_{积分下限}^{积分上限}{被积表达式}`
例如:
`$$ \int_{0}^{1}{x^{3}}dx $$`
显示:

$$\int_{0}^{1}{x^{3}}dx$$

### 7.极限运算
使用`\lim_{变量 \to 表达式} 表达式`

例如:
`$$ \lim_{x \to \infty} \frac{1}{n(n+1)} $$`

显示:

$$\lim_{x \to \infty} \frac{1}{n(n+1)}$$

### 8.累加、累乘

#### 累加

使用` \sum_{下标表达式}^{上标表达式} {累加表达式}`

例如:
`$$ \sum_{i=0}^{n} x_i $$`
显示:

$$\sum_{i=0}^{n} x_i$$

与累加类似:

* 累乘使用`$\prod_$`

$\prod_{i=0}^{n} x_i$

* 并集使用`$\bigcup_$`

* 交集使用`$\bigcap_$`

例如:
`$$ \sum_{i=1}^{n} \frac{1}{i^2} \quad and \ quad \prod_{i=1}^n \frac{1}{i^2} \quad and \quad \bigcup_{i=1}^{2} \Bbb{R} $$`
显示:

$$\sum_{i=1}^{n} \frac{1}{i^2} \quad and \quad \prod_{i=1}^n \frac{1}{i^2} \quad and \quad \bigcup_{i=1}^{2} \Bbb{R}$$

### 9.希腊字母

输入`\小写希腊字母英文全称` 和 `\首字母大写希腊字母英文全称` 来分别输入小写和大写希腊字母

显示(小写)|代码(小写)|显示(大写)|代码(大写)
-|-|-|-
$\alpha$|\$ \alpha \$|$A$|\$ A \$
$\beta$|\$ \beta \$|$B$|\$ B \$
$\gamma$|\$ \gamma \$|$\Gamma$|`$\Gamma$`
$\delta$|\$ \delta \$|$\Delta$|\$\ Delta \$
$\epsilon$|\$ \epsilon \$|$E$|`$E$`
$\zeta$|\$ \zeta \$|$Z$|\$ Z \$
$\eta$|\$ \eta \$|$H$|\$ H \$
$\theta$|\$ \theta \$|$\Theta$|\$ \Theta \$
$\iota$|\$ \iota \$|$I$|\$ I \$
$\kappa$|\$ \kappa \$|$K$|\$ K \$
$\lambda$|\$ \lambda \$|$\Lambda$|\$ \Lambda \$
$\mu$|\$ \mu \$|$M$|\$ M \$
$\nu$|\$ \nu \$|$N$|\$ N \$
$\xi$|\$ \xi \$|$\Xi$|\$ \Xi \$
$o$|\$ o \$|$O$|\$ O \$
$\pi$|\$ \pi \$|$\Pi$|\$ \Pi \$
$\rho$|\$ \rho \$|$R$|\$ R \$
$\sigma$|\$ \sigma \$|$\Sigma$|\$ \Sigma \$
$\tau$|\$ \tau \$|$T$|\$ T \$
$\upsilon$|\$ \upsilon \$|$\Upsilon$|\$ \Upsilon \$
$\phi$|\$ \phi \$|$\Phi$|\$ \Phi \$
$\chi$|\$ \chi \$|$X$|\$ X \$
$\psi$|\$ \psi \$|$\Psi$|\$ \Psi \$
$\omega$|\$ \omega \$|$\Omega$|\$ \Omega \$

### 10.关系运算符

显示|代码
-|-
$\pm$|\$ \pm \$
$\times$|\$ \times \$
$\div$|\$ \div \$
$\mid$|\$ \mid \$
$\nmid$|\$ \nmid \$
$\cdot$|\$ \cdot \$
$\circ$|\$ \circ \$
$\ast$|\$ \ast \$
$\bigodot$|\$ \bigodot \$
$\bigoplus$|\$ \bigoplus \$
$\leq$|\$ \leq \$
$\geq$|\$ \geq \$
$\neq$|\$ \neq \$
$\approx$|\$ \approx \$
$\equiv$|\$ \equiv \$
$\sum$|\$ \sum \$
$\prod$|\$ \prod \$
$\coprod$|\$ \coprod \$
$\backslash$|\$ \backslash \$

### 11.集合运算

显示|代码|描述
-|-|-
$\emptyset$|\$ \emptyset \$|空集
$\in$|\$ \in \$|属于
$\notin$|\$ \notin \$|不属于
$\subset$|\$ \subset \$|真包含于
$\supset$|\$ \supset \$|真包含
$\subseteq$|\$ \subseteq \$|包含于
$\supseteq$|\$ \supseteq \$|包含
$\cap$|\$ \cap \$|交集
$\cup$|\$ \cup \$|并集
$\vee$|\$ \vee \$|
$\wedge$|\$ \wedge \$|
$\uplus$|\$ \uplus \$|
$\top$|\$ \top \$|
$\bot$|\$ \bot \$|
$\complement$|\$ \complement \$|

### 12.对数运算

显示|代码
-|-
$\log$|\$ \log \$
$\lg$|\$ \lg \$
$\ln$|\$ \ln \$

### 13.三角运算

显示|代码
-|-
$\backsim$|\$ \backsim \$
$\cong$|\$ \cong \$
$\angle X$|\$ \angle X \$
$\sin$|\$ \sin \$
$\cos$|\$ \cos \$
$\tan$|\$ \tan \$
$\csc$|\$ \csc \$
$\sec$|\$ \sec \$
$\cot$|\$ \cot \$

### 14.微积分运算

显示|代码
-|-
$\int$|\$ \int \$
$\iint$|\$ \iint \$
$\iiint$|\$ \iiint \$
$\partial$|\$ \partial \$
$\oint$|\$ \oint \$
$\prime$|\$ \prime \$
$\lim$|\$ \lim \$
$\infty$|\$ \infty \$
$\nabla$|\$ \nabla \$

### 15.逻辑运算

显示|代码|描述
-|-|-
$\because$|\$ \because \$|因为
$\therefore$|\$ \therefore \$|所以
$\neg$|\$ \neg \$|非
$\forall$|\$ \forall \$|任意
$\exists$|\$ \exists \$|存在
$\not\subset$|\$ \not\subset \$|不包含于
$\not<$|\$ \not< \$|不小于
$\not>$|\$ \not> \$|不大于
$\not=$|\$ \not= \$|不等于

### 16.戴帽运算

显示|代码
-|-
$\hat{xy}$|\$ \hat{xy} \$
$\widehat{xyz}$|\$ \widehat{xyz} \$
$\bar{y}$|\$ \bar{y} \$
$\tilde{xy}$|\$ \tilde{xy} \$
$\widetilde{xyz}$|\$ \widetilde{xyz} \$
$\acute{y}$|\$ \acute{y} \$
$\breve{y}$|\$ \breve{y} \$
$\check{y}$|\$ \check{y} \$
$\grave{y}$|\$ \grave{y} \$
$\dot{x}$|\$ \dot{x} \$
$\ddot{x}$|\$ \ddot{x} \$

### 17.为公式加注释

使用 `\text{注释内容}`

$f(x)=\begin{cases}0,&\text{if x is even}\\\\1,&\text{if x is odd}\end{cases}$

`$f(x)= \begin{cases} 0,& \text{if x is even} \\\\ 1, & \text{if x is odd} \end{cases}`$

### 18.为公式加序号

使用`\tag{公式序号}`

$$y=ax+b \tag{式1}$$
代码:

\$\$ y=ax+b \tag{式1} $$

### 19.加粗

* 数字加粗:
使用`$\mathbf{数学符号}$`

显示|代码
-|-
$\mathbf{012345679}$|\$ \mathbf{012345679} \$

* 希腊字母加粗:
使用`$\pmb{希腊字母}$`

显示|代码
-|-
$\boldsymbol{\alpha\beta}$|\$ \boldsymbol{\alpha\beta} \$

### 20.矩阵

使用`$$\begin{matrix}...\end{matrix}$$`来实现矩阵:

$\begin{matrix} 1&2&3 \\\\ 4&5&6 \end{matrix}$

`$\begin{matrix} 1&2&3 \\\\ 4&5&6 \end{matrix}$`


$$
  \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
$$

```
$$
  \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
$$
```

* 带{}的矩阵

$$
    \left{
        \begin{matrix}
        1&2&3 \\
        4&5&5 \\
        7&8&9 
        \end{matrix}
    \right} \tag{1}
$$

代码:
```
$$
    \left{
        \begin{matrix}
        1&2&3 \\
        4&5&5 \\
        7&8&9 
        \end{matrix}
    \right} \tag{1}
$$
```

* 带[]的矩阵

$$
    \left[
        \begin{matrix}
        1&2&3 \\
        4&5&6 \\
        7&8&9
        \end{matrix}
    \right] \tag{2}
$$

代码:
```
$$
    \left[
        \begin{matrix}
        1&2&3 \\
        4&5&6 \\
        7&8&9
        \end{matrix}
    \right] \tag{2}
$$
```

* 带省略号的矩阵

$$
\left[
    \begin{matrix}
    1 & 2 & \cdots & 4 \\
    7 & 6 & \cdots &5 \\
    \vdots & \vdots & \ddots & \vdots \\
    8 & 9 & \cdots & 0 \\
    \end{matrix}
\right] \tag{3}
$$

代码:
```
$$
\left[
    \begin{matrix}
    1 & 2 & \cdots & 4 \\
    7 & 6 & \cdots &5 \\
    \vdots & \vdots & \ddots & \vdots \\
    8 & 9 & \cdots & 0 \\
    \end{matrix}
\right] \tag{3}
$$
```

### 21.乘积

* 叉乘:

显示|代码
-|-
$a \times b$|\$ a \times b \$

* 点乘：

显示|代码
-|-
$a \cdot b$|\$ a \cdot b \$

* 内积:

显示|代码
-|-
$\langle a,b \rangle$|\$ \langle a,b \rangle \$

* 外积：

显示|代码
-|-
$a \otimes b$|\$ a \otimes b \$

### 实数R

显示|代码
-|-
$\mathbb{R}$|\$ \mathbb{R} \$

参考资料:
<a href="https://blog.csdn.net/qq_38253837/article/details/109923758">Markdown 数学公式<a/>













