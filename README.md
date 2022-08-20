# ${\LaTeX}$ 快速入门



[TOC]

## 希腊字母

$$
\delta,\lambda\\
\Delta,\Lambda\\
\Alpha\Beta\\
\phi,\varphi\\
\epsilon,\varepsilon\\
π
$$

| 小写       | 大写       | Latex命令                                |
| ---------- | ---------- | ---------------------------------------- |
| $\alpha$   | $\Alpha$   | \alpha                                   |
| $\beta$    | $\Beta$    | \beta                                    |
| $\gamma$   | $\Gamma$   | \gamma                                   |
| $\delta$   | $\Delta$   | \delta                                   |
| $\epsilon$ | $\Epsilon$ | \epsilon（\varepsilon对应$\varepsilon$） |
| $\zeta$    | $\Zeta$    | \zeta                                    |
| $\nu$      | $\Nu$      | \nu                                      |
| $\xi$      | $\Xi$      | \xi                                      |
| $\omicron$ | $\Omicron$ | \omicron                                 |
| $\pi$      | $\Pi$      | \pi                                      |
| $\rho$     | $\Rho$     | \rho                                     |
| $\sigma$   | $\Sigma$   | \sigma                                   |
| $\eta$     | $\Eta$     | \eta                                     |
| $\theta$   | $\Theta$   | \theta                                   |
| $\iota$    | $\Iota$    | \iota                                    |
| $\kappa$   | $\Kappa$   | \kappa                                   |
| $\lambda$  | $\Lambda$  | \lambda                                  |
| $\mu$      | $\Mu$      | \mu                                      |
| $\tau$     | $\Tau$     | \tau                                     |
| $\upsilon$ | $\Upsilon$ | \upsilon                                 |
| $\phi$     | $\phi$     | \phi（\varphi对应$\varphi$）             |
| $\chi$     | $\Chi$     | \chi                                     |
| $\psi$     | $\Psi$     | \psi                                     |
| $\omega$   | $\Omega$   | \omega                                   |

如果使用斜体大写希腊字母,再在大写希腊字母的**LaTeX**命令前加上**var**

## 上下标

$$
a^2,a_1\\
x^{y+z},p_{ij},p_ij\\
x_i,x_{\rm i}\\
\text{A B},\rm{A B}\\
\text A B,\rm A B\\
{\rm A} B\\
\text{e},\text{i}\\
$$

1. 上标`^`,下标`_`
2. 如果上下标多于一个字母,则需要用花括号括起来,如`p_{ij}`
3. 英文字母只有在表示变量(或单一字符的函数名称,如f(x))时才可使用斜体,其余情况都应使用罗马体(直立体).
   - $x_i$: 斜体 i 表示1,2,...,n,为变量
   - $x_{\text i}$: 直立体 i 表示"输入"(input)之意,为普通文本,则需要使用`{\text i}` 或 `{\rm i}`
4. rm和text的区别
   - text 会显示空格,而rm不会
   - text只会让后面第一个字母变成直立体,而rm则会让后面所有字母变成直立体
5. 要让rm只直立一个字母,用`{\rm A} B`
6. 自然对数的底数e,虚数单位ij都应该用直立体

## 分式与根式

$$
\frac{1}{2},\frac 1 2,\\
\frac 1 {x+y}\\
\frac {\dfrac 1 x + 1}{y + 1}
$$

$$
\sqrt 2,\sqrt{x+y},\sqrt[3]x
$$

1. 分式` \frac 1 2`  
2. 当分式分子分母有多个字符时,用大括号框起来` \frac 1 {x+y}`
3. 分式嵌套时,如果希望字体大小保持不变,用`dfrac`,如:`\frac {\dfrac 1 x + 1}{y + 1} `
4. 平方根`\sqrt 2`,n次方根用`\sqrt[3]x` 

## 普通运算符

$$
+-\\
\times,\cdot,\div\\
\pm,\mp\\
><,\ge,\le,\gg,\ll,\ne,\approx,\equiv\\
\cap,\cup,\in,\notin,\subseteq,\subsetneqq,\varnothing\\
\forall,\exists,\nexists\\
\because,\therefore\\
\mathbb R,\R,\Q,\N,\Z_+\\
\mathcal F,\mathscr F
$$

1. 加减`+-`
2. 乘`\times`,点乘`\cdot`,除`\div`
3. 正负号`\pm`(plus-minus),负正号`\mp`(minus-plus)
4. 大于小于`<>`,大于等于`\ge`(greater than or equal),小于等于`\le`(less than or equal),远大于`\gg`,远小于`\ll`,不等于`\ne`(not equal),约等于`\approx`(approximate),恒等于`\equiv`(equivalent)
5. 交集`\cap`,并集`\cup`,属于`\in`,不属于`\notin`,子集`\subseteq`,真子集`\subsetneqq`,空集`\varnothing`
6. 任意`\forall`,存在`\exists`,不存在`\nexists`
7. 因为`\because`,所以`\therefore`
8. 实数集`\mathbb`(blackboard bold)或`\R`(有的编辑器可能不支持),其它数集`\Q` `\N` `\Z_+`
9. 花体字母
   - 傅里叶变换`\mathcal F`(calligraphy,书法),或`\mathscr F`



---



$$
\cdots,\vdots,\ddots
$$

省略号`\cdots`,纵向省略号`\vdots`(vertical),斜向省略号`\ddots`(diagonal,对角的)



---



$$
\infty,\partial,∂,\nabla,\propto,\degree
$$

无穷`\infty`(infinity,无穷)

偏微分符号`\partial`

拉普拉斯算子`\nabla`

正比于`\propto`(proportional to,正比于)

度`\degree`



---


$$
\sin x,\sec x,\cosh x\\
\log_2 x, \ln x,\lg x\\
\lim_{x \to 0} \frac {x}{\sin x}\\
\max x
$$



```latex
\sin x,\sec x,\cosh x
\log_2 x, \ln x,\lg x
\lim_{x \to 0} \frac {x}{\sin x}
\max x
```

因为部分编辑器`\lim_{x \to 0} \frac {x}{\sin x}`极限条件可能会出问题,所以可以使用`\limits`强制让它在下方,如`\lim\limits_{x \to 0} \frac {x}{\sin x}`

## 大型运算符

$$
\sum,\prod\\
\sum_i,\sum_{i=0}^N\\
\frac{\sum\limits_{i=1}^n x_i}{\prod\limits_{i=1}^n x_i}
$$



1. 求和`\sum`,求积`\prod`(product,乘积)
2. `\sum_i`,`\sum_{i=0}^N`
3. `\frac{\sum\limits_{i=1}^n x_i}{\prod\limits_{i=1}^n x_i}`



---


$$
\int,\iint,\iiint,\oint,\oiint\\
\int_{-\infty}^0 f(x)\,\text d x
$$



1. 积分`\int`,二重积分`\iint`,三重积分`\iiint`,环路积分`\oint`,环路二重积分`\oiint`
2. `\int_{-\infty}^0 f(x)\,\text d x`
   - d要用直立体,所以有`\text`
   - d和fx要拉开距离,所以用`\,`



---


$$
a\, a\\
a\ a\\
a\quad a\\
a\qquad a
$$

从上往下按照空格间距排序:

```
a\, a\\
a\ a\\
a\quad a\\
a\qquad a
```



## 标注符号

$$
\vec x,\overrightarrow {AB}\\
\bar x,\overline{AB}
$$

1. 向量`\vec`,多个字母的向量`\overrightarrow`
2. 模长`\bar`,多个字母的模长`\overline`

## 箭头

$$
\leftarrow,\Rightarrow,\Leftrightarrow,\longleftarrow
$$

1.单线箭头`\leftarrow` `\rightarrow`

2.双线箭头`\Leftarrow` `\Rightarrow`

3.长箭头`\longleftarrow`

## 括号与定界符

$$
([])\{ \}\\
\lceil,\rceil,\lfloor,\rfloor,||\\
\left(0,\frac 1 a\right]\\
\left.\frac {∂f}{∂x}\right|_{x=0}
$$

```latex
([])\{ \}\\
\lceil,\rceil,\lfloor,\rfloor,||\\
\left(0,\frac 1 a\right]\\
\left.\frac {∂f}{∂x}\right|_{x=0}
```

1. `\left(`和`\right]`可以随着式子高度自动调整
2. `\right|`高度自适应要在前面加上`\left.`(虚假的括号)



## 多行公式

$$
\begin{align}

a&=b+c+d\\
&=e+f

\end{align}
$$

```latex
\begin{align}

a&=b+c+d\\
&=e+f

\end{align}
```

1. 左对齐`\begin{align}` `\end{align}`
2. `&`(ampersand)表示在括号处对齐

## 大括号

$$
f(x)=

\begin{cases}

\sin x, & -π\le x \le π\\
0,& \text{其他}

\end{cases}
$$



## 矩阵

$$
\begin{matrix}

a & b & \cdots & c \\
\vdots& \vdots & \ddots & \vdots \\
e & f& \cdots & g

\end{matrix}
$$



```latex
\begin{matrix}

a & b & \cdots & c \\
\vdots& \vdots & \ddots & \vdots \\
e & f& \cdots & g

\end{matrix}
```



---


$$
\begin{bmatrix}

a & b & \cdots & c \\
\vdots& \vdots & \ddots & \vdots \\
e & f& \cdots & g

\end{bmatrix}

\begin{pmatrix}

a & b & \cdots & c \\
\vdots& \vdots & \ddots & \vdots \\
e & f& \cdots & g

\end{pmatrix}

\begin{vmatrix}

a & b & \cdots & c \\
\vdots& \vdots & \ddots & \vdots \\
e & f& \cdots & g

\end{vmatrix}
$$

同样的,只需要把`matrix`分别改成`bmatrix` `pmatrix` `vmatrix`即可得到不同样式的矩阵(行列式)

---


$$
\bf A,\bf B^{\rm T}
$$

```
\bf A,\bf B^{\rm T}
```

1. 粗体表示矩阵,`\bf`(bold face,粗体)
2. 转置符号要用直立体

## 实战演练

$$
f(x) = \frac 1 {\sqrt{2\pi} \sigma} {\rm e} ^ {-\frac {(x-\mu)^2}{2\sigma ^ 2}}\\
f(x) = \frac 1 {\sqrt{2\pi} \sigma} \exp \left[ {-\frac {(x-\mu)^2}{2\sigma ^ 2}}\right]
$$

```latex
f(x) = \frac 1 {\sqrt{2\pi} \sigma} {\rm e} ^ {-\frac {(x-\mu)^2}{2\sigma ^ 2}}\\
f(x) = \frac 1 {\sqrt{2\pi} \sigma} \exp \left[ {-\frac {(x-\mu)^2}{2\sigma ^ 2}}\right]
```



---


$$
\lim\limits_{N\to \infty} P \left\{ \left| \frac {I\left( \alpha_i \right)}{N} - H(s) \right| < \varepsilon  \right\} = 1
$$

```latex
\lim\limits_{N\to \infty} P \left\{ \left| \frac {I\left( \alpha_i \right)}{N} - H(s) \right| < \varepsilon  \right\} = 1
```



---


$$
x(n) = \frac 1 {2\pi} \int _{-π} ^ π X\left( {\rm e} ^ {{\rm j} \omega } \right) {\rm e} ^ {{\rm j} \omega n} \, {\rm d}\omega\\
$$

```latex
x(n) = \frac 1 {2\pi} \int _{-π} ^ π X\left( {\rm e} ^ {{\rm j} \omega } \right) {\rm e} ^ {{\rm j} \omega n} \, {\rm d}\omega\\
```



---


$$
\begin{align}

\vec B \left( \vec r \right) &= \frac {\mu_0}{4\pi}\oint_C \frac {I \, {\rm d} \vec l \times \vec R}{R^3}\\

&= \frac {\mu_0}{4\pi} \int_V \frac{\vec J_V \times \vec R}{R^3}\, {\rm d} V'

\end{align}
$$

```latex
\begin{align}

\vec B \left( \vec r \right) &= \frac {\mu_0}{4\pi}\oint_C \frac {I \, {\rm d} \vec l \times \vec R}{R^3}\\

&= \frac {\mu_0}{4\pi} \int_V \frac{\vec J_V \times \vec R}{R^3}\, {\rm d} V'

\end{align}
```

需要注意的是,印刷体表示向量用粗体,所以这里把`\vec`改成`\mathbf`会更好

## 参考资料

1.视频[LaTeX公式保姆级教程 (以及其中的各种细节)](https://www.bilibili.com/video/BV1no4y1U7At/)

2.文件[latex中文手册](https://c7f49cfdf594b0ba.oss-cn-hangzhou.aliyuncs.com/latex%E4%B8%AD%E6%96%87%E6%89%8B%E5%86%8C.pdf)

# LaTeX_Introduction
