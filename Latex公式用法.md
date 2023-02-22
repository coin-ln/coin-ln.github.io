# Latex 公式大全
**/quad 或/qquad表示空格**
## 行内公式

$ f(x)=a+b $  

` $ f(x)=a+b $ `  

## 行间公式

$$ f(x)=a+b $$  

` $$ f(x)=a+b $$ `  

## 手动编号
**命令：\tag{n}表示编号**  

$$ f(x) = a - b \tag{1.1} $$  

`$$ f(x) = a - b \tag{1.1} $$`  

## 简单运算
**命令:\cdot表示乘法的圆点，命令\neq表示不等号，命令\equiv表示恒等于，命令\bmod表示取模**  

$$ x+2-3*4/6=4/y+x \cdot y$$  

`$$ x+2-3*4/6=4/y+x \cdot y$$`  

$$ 0 \neq 1 \quad x \equiv x \quad 1=9 \bmod 2 $$  

`$$ 0 \neq 1 \quad x \equiv x \quad 1=9 \bmod 2 $$`  

## 上下标
**命令：_表示下标，^表示上标,’表示求导,’’表示二阶导**  

$$ a_{ij}^{2}+b^3_{2}=x^{t}+y’+x’’_{12} $$  

`$$ a_{ij}^{2}+b^3_{2}=x^{t}+y’+x’’_{12} $$`  

## 根号、分式
**命令：\sqrt表示平方根，\sqrt[n]表示n次方根，\frac表示分式**  

$$ \sqrt{x}+\sqrt{x^{2}+\sqrt{y}}=\sqrt[3]{k_{i}}-\frac{x}{m} $$  

`$$ \sqrt{x}+\sqrt{x^{2}+\sqrt{y}}=\sqrt[3]{k_{i}}-\frac{x}{m} $$`  

## 上下标记
**命令：\overline, \underline 分别在表达式上、下方画出水平线**  

$$ \overline{x+y} \qquad \underline{a+b} $$  

`$$ \overline{x+y} \qquad \underline{a+b} $$` 

**命令：\overbrace, \underbrace 分别在表达式上、下方给出一个水平的大括号**  

$$ \overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26} $$

`$$ \overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26} $$`  

## 向量
**命令：\vec表示向量，\overrightarrow表示箭头向右的向量，\overleftarrow表示箭头向左的向量**  

$$ \vec{a}+\overrightarrow{AB}+\overleftarrow{DE}$$

`$$ \vec{a}+\overrightarrow{AB}+\overleftarrow{DE}$$`  

## 积分、极限、求和、乘积
**命令：\int表示积分，\lim表示极限， \sum表示求和，\prod表示乘积，^、_表示上、下限**  

$$ \lim_{x \to \infty} x^2_{22} - \int_{1}^{5}x\mathrm{d}x+\sum_{n=1}^{20} n^{2}=\prod_{j=1}^{3} y_{j} +\lim_{x\to-2} \frac{x-2}{x} $$  

`$$ \lim_{x \to \infty} x^2_{22} - \int_{1}^{5}x\mathrm{d}x+\sum_{n=1}^{20} n^{2}=\prod_{j=1}^{3} y_{j} +\lim_{x\to-2} \frac{x-2}{x} $$`  

## 三圆点
**命令：\ldots点位于基线上，\cdots点设置为居中，\vdots使其垂直，\ddots对角线排列**  

$$ x_{1},x_{2},\ldots,x_{5}  \quad x_{1} + x_{2} + \cdots + x_{n} $$  

`$$ x_{1},x_{2},\ldots,x_{5}  \quad x_{1} + x_{2} + \cdots + x_{n} $$`  

## 重音符号

$$ \hat{x} $$   

`$$ \hat{x} $$`  

$$ \bar{x} $$  

`$$ \bar{x} $$`  

$$ \tilde{x} $$  

`$$ \tilde{x} $$`  

## 矩阵

![](datas/Matrix%20format.jpg)  

下列代码中，&用于分隔列，\用于分隔行  

$$\begin{bmatrix}
1 & 2 & \cdots \\
67 & 95 & \cdots \\
\vdots  & \vdots & \ddots \\
\end{bmatrix}$$  

```
$$\begin{bmatrix}
1 & 2 & \cdots \\
67 & 95 & \cdots \\
\vdots  & \vdots & \ddots \\
\end{bmatrix}$$
```  

## 希腊字母

![](datas/greek%20alphabet.jpg)  

$$ \alpha^{2} + \beta =\Theta $$   

`$$ \alpha^{2} + \beta =\Theta $$`  

## 多行公式
### 1.公式组合

$$ D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases} $$  

```
$$D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases}$$
```

### 2.拆分单个公式

$$ \begin{split}
\cos 2x &= \cos^2x - \sin^2x \\
&=2\cos^2x-1
\end{split} $$  

```
$$\begin{split}
\cos 2x &= \cos^2x - \sin^2x \\
&=2\cos^2x-1
\end{split}$$
```


