> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [zhuanlan.zhihu.com](https://zhuanlan.zhihu.com/p/457858293)


## 00 - 序言

对于这个科目而言，你能做的是形成正确的**几何直观**

## 01 - 向量究竟是什么

> 引入一些数作为坐标是一种鲁莽的行为。——赫尔曼 · 外尔


1. 三种看待向量的观点
| 物理专业的学生 | 空间中的箭头（长度和方向） |
| --- | --- |
| 计算机专业的学生 | 有序的数字列表 |
| 数学家 | 任何东西（以上两个观点的碰撞） |


2. 思考向量的特定方式

线性代数围绕两种基本运算：**向量加法**和**向量数乘**

|  | 物理观点 | 列表观点 |
| --- | --- | --- |
| 向量的加法 | 运动 | 对应项相加 |
| 向量的数乘 | 缩放（标量的作用就是缩放） | 分量与标量相乘 |


## 02 - 线性组合 张成的空间与基

eg. $\begin{bmatrix} 3\\-2 \end{bmatrix} = 3\hat{i}+(-2)\hat{j}$

**基向量**： $\hat{i},\hat{j}$ 被称作**基向量**，是**缩放的对象**

$a\vec{v}+b\vec{w}$

**线性组合**：两个数乘向量的和被称为这两个向量的**线性组合**

$\left\{ a\vec{v}+b\vec{w}\mid a,b\in\mathbb{R}\right\}$

**张成的空间**：所有可以表示为给定向量**线性组合**的向量的**集合**被称为给定向量**张成的空间**

二维

| 给定的二维向量 | 张成的空间 |
| --- | --- |
| 一般的两个二维向量 | 所有二维向量的集合 |
| 两个共线的向量 | 一条直线上的向量的集合 |
| 两个零向量 | 一个点 |


三维

| 给定的向量 | 张成的空间 |
| --- | --- |
| 一般的两个向量 | 过原点的平面 |
| 三个向量，第三个落在前两个所张成的平面上 | 平面 |
| 一般的三个向量 | 空间中所有的三维向量（平面的扫动） |


**线性相关**：有多个向量，可以移除之一而不减小张成的空间，称它们是**线性相关**的

反之，所有向量都给张成的空间增加新的维度，

$\vec{u}\ne a\vec{c}+b\vec{w}$

称它们是**线性无关**的

**向量空间的一组基**（严格定义）：**向量空间的一组基**是张成该空间的一个**线性无关**的向量集

## 03 - 矩阵与线性变换

1.“**变换**” 本质上是 “**函数**” 的一种花哨的说法（向量输入和向量输出）；“**变换**” 暗示用 “**运动**” 的观点思考

2.  **线性变换**：①**任意**直线→直线②原点不变（保持网格线平行且等距分布的变换） 
3.  用数值描述线性变换，考虑 $\hat{i},\hat{j}$ 的变换，可以确定任意向量的变换；一个二维线性变换仅由四个数字完全确定，即基向量的变换 

4.2×2 矩阵，列理解为两个特殊向量，即变换后的 $\hat{i},\hat{j}$

eg. 变换 $\begin{bmatrix} 3&2\\ -2&1 \end{bmatrix}$ ，则 $\begin{bmatrix} 5\\ 7 \end{bmatrix}\rightarrow 5\begin{bmatrix} 3\\ -2 \end{bmatrix}+ 7\begin{bmatrix} 2\\ 1 \end{bmatrix}= \begin{bmatrix} 29\\ -3 \end{bmatrix}$

一般， $\begin{bmatrix} a&b\\ c&d \end{bmatrix}$ ，则 $\begin{bmatrix} x\\ y \end{bmatrix}\rightarrow x\begin{bmatrix} a\\ c \end{bmatrix}+ y\begin{bmatrix} b\\ d \end{bmatrix}= \begin{bmatrix} ax+by\\ cx+dy \end{bmatrix}$

5. 定义矩阵乘法

$\begin{bmatrix} a&b\\ c&d \end{bmatrix} \begin{bmatrix} x\\ y \end{bmatrix}= x\begin{bmatrix} a\\ c \end{bmatrix}+ y\begin{bmatrix} b\\ d \end{bmatrix}= \begin{bmatrix} ax+by\\ cx+dy \end{bmatrix}$

## 04 - 矩阵乘法与线性变换复合

1. **旋转**与**剪切**的 “复合变换”

eg.

$\begin{bmatrix} 1&1\\ 0&1 \end{bmatrix} \pmatrix{ \begin{bmatrix} 0&1\\ 1&0 \end{bmatrix} \begin{bmatrix} x\\ y \end{bmatrix}}= \begin{bmatrix} 1&-1\\ 1&0 \end{bmatrix} \begin{bmatrix} x\\ y \end{bmatrix}$

其中 $\begin{bmatrix} 0&-1\\ 1&0 \end{bmatrix}$ 为旋转矩阵，$\begin{bmatrix} 1&1\\ 0&1 \end{bmatrix}$ 为剪切矩阵， $\begin{bmatrix} 1&-1\\ 1&0 \end{bmatrix}$ 为复合矩阵

$\therefore \begin{bmatrix} 1&1\\ 0&1 \end{bmatrix} \begin{bmatrix} 0&-1\\ 1&0 \end{bmatrix}= \begin{bmatrix} 1&-1\\ 1&0 \end{bmatrix}$

两个矩阵相乘有着几何意义，也就是**两个线性变换相继作用**

2. 矩阵的乘法

eg.

$M_1=\begin{bmatrix} 1&-2\\ 1&0 \end{bmatrix}, M_2=\begin{bmatrix} 0&2\\ 1&0 \end{bmatrix}, M_2 M_1= \begin{bmatrix} 0&2\\ 1&0 \end{bmatrix} \begin{bmatrix} 1&-2\\ 1&0 \end{bmatrix}=?$

Where does $\hat{i}$ go?

$\begin{bmatrix} 0&2\\ 1&0 \end{bmatrix} \begin{bmatrix} 1\\ 1 \end{bmatrix}= \begin{bmatrix} 2\\ 1 \end{bmatrix}$

类似地， $\hat{j}$

$\begin{bmatrix} 0&2\\ 1&0 \end{bmatrix} \begin{bmatrix} -2\\ 0 \end{bmatrix}= \begin{bmatrix} 0\\ -2 \end{bmatrix}$

$\therefore M_2 M_1= \begin{bmatrix} 0&2\\ 1&0 \end{bmatrix} \begin{bmatrix} 1&-2\\ 1&0 \end{bmatrix}= \begin{bmatrix} 2&0\\ 1&-2 \end{bmatrix}$

一般，

$\begin{bmatrix} a&b\\ c&d \end{bmatrix} \begin{bmatrix} e&f\\ g&h \end{bmatrix} = \begin{bmatrix} ae+bg&af+bh\\ ce+dg&cf+dh \end{bmatrix}$

3. **矩阵乘法交换律不成立**

$M_1 M_2\ne M_2 M_1$

4. **矩阵乘法结合律成立**

$(AB)C=A(BC)$

## 附注 1 - 三维空间中的线性变换

## 05 - 行列式

1. 行列式

**行列式**：线性变换**改变面积的比例**（由于网格线平行等距，对任意图形缩放比例相等）被称为这个变换的**行列式**

eg. ${\rm det}\pmatrix{\begin{bmatrix} 3&2\\ 0&2 \end{bmatrix}}=6$

2.  行列式的正负与平面的取向有关；行列式为负，空间被翻转；三维翻转，右手系变为左手系 
3.  行列式的计算 

${\rm det}\pmatrix{\begin{bmatrix} a&b\\ c&d \end{bmatrix}} =ad-bc$

![](https://pic4.zhimg.com/v2-73f5933ea50afddc59797a1369faaaf7_r.jpg#crop=0&crop=0&crop=1&crop=1&id=HExKh&originHeight=340&originWidth=720&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

${\rm det}\pmatrix{\begin{bmatrix} a&b&c\\ d&e&f\\ g&h&i \end{bmatrix}}= a\ {\rm det}\pmatrix{\begin{bmatrix} e&f\\ h&i \end{bmatrix}} -b\ {\rm det}\pmatrix{\begin{bmatrix} d&f\\ g&i \end{bmatrix}} +c\ {\rm det}\pmatrix{\begin{bmatrix} d&e\\ g&h \end{bmatrix}}$

## 06 - 逆矩阵、列空间与零空间

1. 线性方程组与向量方程

eg.

$\begin{equation} \begin{array}{l} 2x+5y+3z=-3\\ 4x+0y+8z=0\\ 1x+3y+0z=2 \end{array} \end{equation}\rightarrow \begin{bmatrix} 2&5&3\\ 4&0&8\\ 1&3&0 \end{bmatrix} \begin{bmatrix} x\\y\\z \end{bmatrix}= \begin{bmatrix} -3\\0\\2 \end{bmatrix}$

$A\vec{x}=\vec{v}$ 其中 $A$ 为系数矩阵， $\vec{x}$ 为包含未知数的向量， $\vec{v}$ 为常数向量

2. 几何解释

$A$ 代表一种线性变换，向量方程意义是找到 $\vec{x}$ 经过变换后与 $\vec{v}$ 重合

3. 方程求解

当 ${\rm det}(A)\ne0$ ， $\vec{x},\vec{v}$ 一一对应； $\vec{v}$ 经过逆变换得 $\vec{x}$

$A$ 的逆记为 $A^{-1}$

$A^{-1}A= \begin{bmatrix} 1&0\\ 0&1 \end{bmatrix}$

$A\vec{x}=\vec{v}\\ A^{-1}A\vec{x}=A^{-1}\vec{v}\\ \therefore \vec{x}=A^{-1}\vec{v}$

当 $det(A)=0$ ，没有逆变换（不能 “解压缩”）；**可能有解**

4. 列空间

**列空间**：所有可能的输出向量 $A\vec{v}$ 构成的集合被称为 $A$ 的**列空间**

列空间就是**矩阵的列所张成的空间**

5. 秩

**秩**：**秩**是**列空间的维数**，代表着变换后空间的维数

eg. 对于 2×2 的矩阵，它的秩最大为 2

**满秩**：秩达到最大值时，意味着秩与列数相等，称之为**满秩**

6. 零空间（核）

零向量一定在列空间中（线性变换必须**保证原点不变**）

对一个满秩变换，唯一能在变换后落在原点的就是零向量

对一个非满秩变换，会有一系列向量变换后成为零向量

**零空间（核）**：**变换后落在原点**的向量的**集合**，被称为矩阵的**零空间**或**核**

对线性方程组 $A\vec{x}=\vec{v}$ ，当 $\vec{v}= \begin{bmatrix} 0\\0 \end{bmatrix}$ 时，零空间给出的就是这个向量方程的**所有解**

7. 总结

以上就是从集合角度理解线性方程组的一个高水平概述

每个方程组都有一个线性变换与之联系

当逆变换存在时，可用逆变换求解方程组

否则，列空间的概念让我们清楚什么时候存在解

零空间的概念有助于理解所有可能的解的集合是什么样的

## 附注 2 - 非方阵

1. 非方阵的几何含义

eg. $\begin{bmatrix} 2&0\\ -1&1\\ -2&1 \end{bmatrix}$ 这个变换将 $\hat{i}$ 变换到坐标 $(2,-1,-2)$ ， $\hat{j}$ 变换到坐标 $(0,1,1)$

![](https://pic2.zhimg.com/v2-1e340b1a02f5d982530ff278367f7c2d_r.jpg#crop=0&crop=0&crop=1&crop=1&id=Utteq&originHeight=389&originWidth=680&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

这个变换是**满秩**的；是二维向三维的映射

## 07 - 点积与对偶性

> 卡尔文：你知道吗，我觉得数学不是一门科学，而是一种宗教。
霍布斯：一种宗教？
卡尔文：是啊。这些公式就像奇迹一般。你取出两个数，把它们相加时，他们神奇地成为了一个全新的数！没人能说清这到底是怎么发生的。你要么完全相信，要么完全不信。


1. 标准观点

eg. $\begin{bmatrix} 1\\2 \end{bmatrix}\cdot \begin{bmatrix} 3\\4 \end{bmatrix}= 1\cdot3+2\cdot4$

![](https://pic1.zhimg.com/v2-1535a06c4964fbf911eeaa2e81fd2cb8_r.jpg#crop=0&crop=0&crop=1&crop=1&id=XkFvW&originHeight=403&originWidth=685&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

2. 为什么点积与顺序无关

如果 $\vec{v},\vec{w}$ 的长度恰好相同，可以利用**对称性**（ $\vec{w}$ 向 $\vec{v}$ 上的投影等于 $\vec{v}$ 向 $\vec{w}$ 上的投影）

如果它们的长度不同，例如 $2\vec{v},\vec{w}$

当 $\vec{w}$ 向 $2\vec{v}$ 上投影， $\vec{w}$ 的投影长度不变，$(2\vec{v})\cdot\vec{w}=2(\vec{v}\cdot\vec{w})$

当 $2\vec{v}$ 向 $\vec{w}$ 上投影， $2\vec{v}$ 的投影长度变为两倍，$(2\vec{v})\cdot\vec{w}=2(\vec{v}\cdot\vec{w})$

即使对称性被破坏，两种理解下，缩放向量对点积结果的影响是相同的

3. 点积和投影的联系：**对偶性**

多维空间到一维空间（数轴）的线性变换

eg. $\begin{bmatrix} 1&-2 \end{bmatrix}\begin{bmatrix} 4\\3 \end{bmatrix}= 4\cdot1+3\cdot(-2)$

$\begin{bmatrix} 1&-2 \end{bmatrix}$ 为变换（看作**倾倒的向量**）， $\begin{bmatrix} 4\\3 \end{bmatrix}$ 为向量

设一数轴的单位向量为 $\hat{u}$

$\hat{i}$ 向 $\hat{u}$ 所在直线的投影与 $\hat{u}$ 向 $x$ 轴投影**完全对称**

对 $\hat{j}$ 同理

$\therefore$ 二维空间向该数轴的线性变换为 $\begin{bmatrix} u_x&u_y \end{bmatrix}$

$\begin{bmatrix} u_x&u_y \end{bmatrix} \begin{bmatrix} x\\y \end{bmatrix}= u_x\cdot x+u_y\cdot y$ （矩阵向量乘积）

$\begin{bmatrix} u_x\\u_y \end{bmatrix} \begin{bmatrix} x\\y \end{bmatrix}= u_x\cdot x+u_y\cdot y$ （点积）

若 $\vec{u}$ 为非单位向量，结合对称性被破坏时的**顺序无关**，同理可得

## 08 第一部分 - 叉积的标准介绍

1. 二维叉积

$\vec{v}\times\vec{w}$ **数值**为它们所张成的**平行四边形的面积**，“**正负**” 由**右手定则**决定；用**行列式**计算

eg. $\vec{v}= \begin{bmatrix} -3\\1 \end{bmatrix} ,\vec{w} =\begin{bmatrix} 2\\1 \end{bmatrix}$

$\vec{v}\times\vec{w}={\rm det}\pmatrix{ \begin{bmatrix} 3&2\\1&1 \end{bmatrix}} =-3\cdot1-2\cdot1=-5$

两个向量所成平行四边形的面积为 5，且因为 $\vec{v}$ 在 $\vec{w}$ 的左侧，结果为负

此外，$\vec{v},\vec{w}$ 越接近垂直，面积越大； $(a\vec{v})\times\vec{w}=a(\vec{v}\times\vec{w})$

2. 真正的叉积

真正的叉积是通过两个三维向量生成一个新的三维向量

$\vec{v}\times\vec{w}=\vec{p}$

$\vec{p}$ 长度为平行四边形的面积，方向于平行四边形所在的面垂直，遵循右手定则

$\begin{bmatrix} v_1\\v_2\\v_3 \end{bmatrix}\times \begin{bmatrix} w_1\\w_2\\w_3 \end{bmatrix}= {\rm det}\pmatrix{\begin{bmatrix} \hat{i}&v_1&w_1\\ \hat{j}&v_2&w_2\\ \hat{k}&v_3&w_3 \end{bmatrix}}$

## 08 第二部分 - 以线性变换的眼光看叉积

1. 回顾

**对偶性**的思想在于，一个空间到数轴的线性变换与空间中唯一一个向量对应，也就是说**应用线性变换与向量点乘等价**

这样的向量被称为这个变换的**对偶向量**

2. 三维空间到数轴的特定线性变换

$f\pmatrix{\begin{bmatrix} x\\y\\z \end{bmatrix}}= {\rm det}\pmatrix{\begin{bmatrix} x&v_1&w_1\\ y&v_2&w_2\\ z&v_3&w_3 \end{bmatrix}}$

这个函数的几何意义是，对于任一输入的向量 $(x,y,z)$ ，输出由它和 $\vec{v},\vec{w}$ 确定的**平行六面体体积**（有正负）

这个函数是**线性的**，因而可以写成矩阵乘法

又因为应用这个变换和与对偶向量点乘等价，所以

$\vec{p}\cdot \begin{bmatrix} x\\y\\z \end{bmatrix}= \begin{bmatrix} p_1\\p_2\\p_3 \end{bmatrix}\cdot \begin{bmatrix} x\\y\\z \end{bmatrix}= {\rm det}\pmatrix{\begin{bmatrix} x&v_1&w_1\\ y&v_2&w_2\\ z&v_3&w_3 \end{bmatrix}}$

$p_1\cdot x+p_2\cdot y+p_3\cdot z= x(v_2\cdot w_3-v_3\cdot w_2)+ y(v_3\cdot w_1-v_1\cdot w_3)+ z(v_1\cdot w_2-v_2\cdot w_1)$

$\begin{equation} \begin{array}{l} p_1=v_2\cdot w_3-v_3\cdot w_2\\ p_2=v_3\cdot w_1-v_1\cdot w_3\\ p_3=v_1\cdot w_2-v_2\cdot w_1 \end{array} \end{equation}$

比较 $\begin{bmatrix} v_1\\v_2\\v_3 \end{bmatrix}\times \begin{bmatrix} w_1\\w_2\\w_3 \end{bmatrix}= \hat{i}(v_2\cdot w_3-v_3\cdot w_2)+ \hat{j}(v_3\cdot w_1-v_1\cdot w_3)+ \hat{k}(v_1\cdot w_2-v_2\cdot w_1)$

3. 什么样的 $\vec{p}$ 满足条件

$p\cdot \begin{bmatrix} x\\y\\z \end{bmatrix}$ 的几何解释是把其他向量向 $\vec{p}$ 投影的长度与 $\vec{p}$ 的长度相乘

平行六面体的体积

= 平行四边形的面积乘 $(x,y,z)$ 垂直于 $\vec{v},\vec{w}$ 的分量

= 垂直于 $\vec{v},\vec{w}$ 且长度为平行四边形面积的向量与 $(x,y,z)$ 点乘

点积为正的情况会与 $(x,y,z),\vec{v},\vec{w}$ 满足右手定则的情况吻合

这就是**叉积的计算**与**几何解释**有关联的根本原因

3. 总结

首先，定义一个三维空间到数轴的线性变换

然后，考虑这个变换的对偶向量

①应用这个变换和与对偶向量点乘等价

②从几何角度思考，这个对偶向量必然与 $\vec{v},\vec{w}$ 垂直，长度等于两个向量张成的平四面积

## 09 - 基变换

1. 坐标系和基向量

**坐标系**：发生在向量与一组数之间的任意一种转化，都被称为一个**坐标系**

其中两个特殊的向量 $\hat{i},\hat{j}$ 被称为这个坐标系的**基向量**

2. 讨论使用另一组基向量的思想

将基向量理解为 “**语言**”

**如何在不同坐标系之间转化？**

eg. 我看 Jenny 的基向量 $\vec{b_1}= \begin{bmatrix} 2\\1 \end{bmatrix} \vec{b_2}= \begin{bmatrix} -1\\1 \end{bmatrix}$

对于同一个向量，我看是 $\begin{bmatrix} 3\\2 \end{bmatrix}$ ，Jenny 看是  $\begin{bmatrix} \frac{5}{3}\\\frac{1}{3} \end{bmatrix}$ （不同的语言描述同一个向量）

Jenny 用 $\begin{bmatrix} -1\\2 \end{bmatrix}$ 表示一个向量，在我们的坐标系如何描述？（如何从她的语言转化到我们的语言？）

$\begin{bmatrix} 2&-1\\1&1 \end{bmatrix} \begin{bmatrix} -1\\2 \end{bmatrix}= -1\begin{bmatrix} 2\\1 \end{bmatrix}+ 2\begin{bmatrix} -1\\1 \end{bmatrix}= \begin{bmatrix} -4\\1 \end{bmatrix}$

$\begin{bmatrix} 2&-1\\ 1&1 \end{bmatrix}$ 从几何上，将我们的网格变换为 Jenny 的网格；从数值上，将她的语言转化为我们的语言（相反的）

把它看作我们对 Jenny 的向量的误解，也就是我们的坐标系有相同坐标的向量，变换成真正想表示的向量

$\begin{bmatrix} 2&-1\\1&1 \end{bmatrix}^{-1}$ 将 Jenny 的网格变换为我们的网格；将我们的语言转化为她的语言

Jenny 如何描述同样的空间 $90^{\circ}$ 旋转？

$\begin{bmatrix} 2&-1\\1&1 \end{bmatrix}\vec{v}$ 转化成我们的语言

$\begin{bmatrix} 0&-1\\1&0 \end{bmatrix} \begin{bmatrix} 2&-1\\1&1 \end{bmatrix}\vec{v}$ 用我们的语言描述变换矩阵

$\begin{bmatrix} 2&-1\\1&1 \end{bmatrix}^{-1} \begin{bmatrix} 0&-1\\1&0 \end{bmatrix} \begin{bmatrix} 2&-1\\1&1 \end{bmatrix}\vec{v}$ 用她的语言描述变换后的向量

表达式 $A^{-1}MA$ 暗示着一种数学上的**转移作用**，中间的矩阵代表**你所见的变换**

## 10 - 特征向量与特征值

1. 特征向量与特征值

满足 $A\vec{v}=\lambda\vec{v}$

将等号右侧重写为某个矩阵向量乘积

$\lambda\vec{v}$ 表示 $\vec{v}$ 的每个基向量与 $\lambda$ 相乘，因此可以重写为 $\begin{bmatrix} \lambda&0&0\\ 0&\lambda&0\\ 0&0&\lambda \end{bmatrix}\vec{v}$

$A\vec{v}=(\lambda I)\vec{v}$

$(A-\lambda I)\vec{v}=\vec{0}$

当且仅当矩阵代表的变换将空间**压缩到更低维度**时，才会存在满足上式的非零向量

$\therefore {\rm det}(A-\lambda I)=0$

二维线性变换不一定有特征向量，如旋转 90 度的变换

2. 特征基与对角化

如果基向量都是特征向量，eg. $\begin{bmatrix} -1&0\\0&2 \end{bmatrix}$

**对角矩阵**：除了对角元以外其他元素均为 0 的矩阵被称为**对角矩阵**

对角矩阵所有的基向量都是特征向量，矩阵的**对角元**是它们**所属的特征值**

用特征向量作为基

eg. $\begin{bmatrix} 3&1\\0&2 \end{bmatrix}$ 取特征向量 $\begin{bmatrix} 1\\0 \end{bmatrix} ,\begin{bmatrix} -1\\1 \end{bmatrix}$ 作为基

$\begin{bmatrix} 1&-1\\0&1 \end{bmatrix}^{-1} \begin{bmatrix} 3&1\\0&2 \end{bmatrix} \begin{bmatrix} 1&-1\\0&1 \end{bmatrix}$ 新矩阵必然是对角的

$\begin{bmatrix} 1&-1\\0&1 \end{bmatrix}^{-1} \begin{bmatrix} 3&1\\0&2 \end{bmatrix} \begin{bmatrix} 1&-1\\0&1 \end{bmatrix}= \begin{bmatrix} 3&0\\0&2 \end{bmatrix}$

**特征基**：一组特征向量作为基向量构成的集合被称为一组**特征基**

计算 $\begin{bmatrix} 3&1\\0&2 \end{bmatrix}^{100}$ ，一种更容易的做法是先变换到特征基，计算 100 次幂，然后转化回标准系

> 解：
计算特征值和特征向量，得特征基变换矩阵 $\begin{bmatrix} 1&-1\\ 0&1 \end{bmatrix}$ ，并求出它的逆 $\begin{bmatrix} 1&-1\\0&1 \end{bmatrix}^{-1}= \begin{bmatrix} 1&1\\ 0&1 \end{bmatrix}$
对角化， $\begin{bmatrix} 1&-1\\0&1 \end{bmatrix}^{-1} \begin{bmatrix} 3&1\\0&2 \end{bmatrix} \begin{bmatrix} 1&-1\\0&1 \end{bmatrix}= \begin{bmatrix} 3&0\\0&2 \end{bmatrix}$
特征基下， $\begin{bmatrix} 3&0\\0&2 \end{bmatrix}^{100}= \begin{bmatrix} 3^{100}&0\\ 0&2^{100} \end{bmatrix}$
回到标准系，得 $\begin{bmatrix} 3&1\\0&2 \end{bmatrix}^{100}= \begin{bmatrix} 1&-1\\0&1 \end{bmatrix} \begin{bmatrix} 3^{100}&0\\0&2^{100} \end{bmatrix} \begin{bmatrix} 1&-1\\0&1 \end{bmatrix}^{-1}= \begin{bmatrix} 3^{100}&3^{100}-2^{100}\\0&2^{100} \end{bmatrix}$


并非所有矩阵都能对角化，如剪切矩阵（特征向量不能张成全空间）

![](https://pic4.zhimg.com/v2-71f972bec56e09362f002eca4bab950b_r.jpg#crop=0&crop=0&crop=1&crop=1&id=nrYSz&originHeight=435&originWidth=727&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

> 解：
$A^2= \begin{bmatrix} 1&1\\1&2 \end{bmatrix}, A^3=\begin{bmatrix} 1&2\\2&3 \end{bmatrix}, A^4=\begin{bmatrix} 2&3\\3&5 \end{bmatrix}, A^5=\begin{bmatrix} 3&5\\5&8 \end{bmatrix}$
猜想 $A^n= \begin{bmatrix} F_{n-1}&F_n\\F_{n}&F_{n+1} \end{bmatrix}$ ，其中 $\{F_n\}$ 为斐波那契数列
证明（数学归纳法）：
$n=1$ 时，猜想成立；
若 $n=k$ 时成立，则
$A^{k+1}=\begin{bmatrix} 0&1\\1&1 \end{bmatrix} \begin{bmatrix} F_{n-1}&F_n\\F_{n}&F_{n+1} \end{bmatrix}= \begin{bmatrix} F_{n}&F_{n+1}\\F_{n-1}+F_{n}&F_{n}+F_{n+1} \end{bmatrix}= \begin{bmatrix} F_{n}&F_{n+1}\\F_{n+1}&F_{n+2} \end{bmatrix}$
符合猜想
QED
解法（特征基）：
特征基变换矩阵 $M=\begin{bmatrix} 2&2\\1+\sqrt{5}&1-\sqrt{5} \end{bmatrix}$ ，求出它的逆 $M^{-1=}\begin{bmatrix} \frac{5-\sqrt{5}}{20}&\frac{\sqrt{5}}{10}\\ \frac{5+\sqrt{5}}{20}&-\frac{\sqrt{5}}{10} \end{bmatrix}$
对角化， $M^{-1}AM= \begin{bmatrix} \frac{1+\sqrt{5}}{2}&0\\ 0&\frac{1-\sqrt{5}}{2} \end{bmatrix}$
$A^n=M \begin{bmatrix} (\frac{1+\sqrt{5}}{2})^n&0\\ 0&(\frac{1-\sqrt{5}}{2})^n \end{bmatrix} M^{-1}= \begin{bmatrix} \frac{1}{\sqrt{5}}\left[ (\frac{1+\sqrt5}{2})^{n-1}-(\frac{1-\sqrt5}{2})^{n-1} \right]& \frac{1}{\sqrt{5}}\left[ (\frac{1+\sqrt5}{2})^{n}-(\frac{1-\sqrt5}{2})^{n} \right]\\ \frac{1}{\sqrt{5}}\left[ (\frac{1+\sqrt5}{2})^{n}-(\frac{1-\sqrt5}{2})^{n} \right]& \frac{1}{\sqrt{5}}\left[ (\frac{1+\sqrt5}{2})^{n+1}-(\frac{1-\sqrt5}{2})^{n+1} \right] \end{bmatrix}$
比较，可得 $F_n=\frac{1}{\sqrt{5}}\left[ (\frac{1+\sqrt5}{2})^{n}-(\frac{1-\sqrt5}{2})^{n} \right]$


## 11 - 抽象向量空间

**行列式**和**特征向量**与所选坐标系无关；这二者都是暗含于空间中的性质

1. 函数实际上只是另一种向量

$(f+g)(x)=f(x)+g(x)$ 和向量对应坐标相加相似（无数个坐标的相加）

$(2f)(x)=2f(x)$ 和向量对应坐标数乘相似

2. 函数的线性变换

函数的线性变换，这个变换接收一个函数，并把它变成另一个函数，例如求导；“**算子**” 和 “**变换**” 是一样的

**线性的严格定义**： $L(\vec{v}+\vec{w})=L(\vec{v})+L(\vec{w}),L(c\vec{v})=cL(\vec{v})$ 【可加性和成比性（一阶齐次）】

一个函数变换是线性的？

eg. 求导是线性运算 $(f(x)+g(x))'=f'(x)+g'(x),(af(x))'=af'(x)$

用矩阵描述求导

当前空间为全体多项式；自然地，取 $1,x,x^2,x^3,\ldots$ 为基（基函数）， $b_0(x)=1,b_1(x)=x,\ldots$ ，基函数集是无穷大的

eg. $1x^2+3x+5\cdot1= \begin{bmatrix} 5\\3\\1\\0\\0\\\vdots \end{bmatrix}$

$a_nx^n+a_{n-1}x^{n-1}+\cdots+a_1x+a_0= \begin{bmatrix} a_0\\a_1\\\vdots\\a_{n-1}\\a_n\\0\\\vdots \end{bmatrix}$

$\frac{\rm d}{{\rm d}x}= \begin{bmatrix} 0&1&0&0&\cdots\\ 0&0&2&0&\cdots\\ 0&0&0&3&\cdots\\ 0&0&0&0&\cdots\\ \vdots&\vdots&\vdots&\vdots&\ddots \end{bmatrix}$

eg. $\frac{\rm d}{{\rm d}x}(1x^3+5x^2+4x+5)= \begin{bmatrix} 0&1&0&0&\cdots\\ 0&0&2&0&\cdots\\ 0&0&0&3&\cdots\\ 0&0&0&0&\cdots\\ \vdots&\vdots&\vdots&\vdots&\ddots \end{bmatrix} \begin{bmatrix} 5\\4\\5\\1\\\vdots \end{bmatrix}= \begin{bmatrix} 1\cdot4\\2\cdot5\\3\cdot1\\0\\\vdots \end{bmatrix}$

| 线性代数中的概念 | 应用于函数时的别名 |
| --- | --- |
| 线性变换 | 线性算子 |
| 点积 | 内积 |
| 特征向量 | 特征函数 |


3. 向量空间

**向量空间**：这些类似向量的事物，比如箭头、一组数、函数等，它们构成的集合被称为**向量空间**

如果要让所有建立好的理论和概念适用于一个向量空间，那么它必须满足八条公理

$\begin{equation} \begin{array}{l} 1)\vec{u}+(\vec{v}+\vec{w})=(\vec{u}+\vec{v})+\vec{w}\\ 2)\vec{v}+\vec{w}=\vec{w}+\vec{v}\\ 3)\vec{0}+\vec{v}=\vec{v}\\ 4)\vec{v}+(-\vec{v})=\vec{0}\\ 5)a(b\vec{v})=ab(\vec{v})\\ 6)1\vec{v}=\vec{v}\\ 7)a(\vec{v}+\vec{w})=a\vec{v}+a\vec{w}\\ 8)(a+b)\vec{v}=a\vec{v}+b\vec{v} \end{array} \end{equation}$

**向量的形式并不重要**，只要向量相加和数乘的概念遵守以上规则即可

> “普适的代价是抽象”Abstractness is the price of generality.


## 12 - 克莱姆法则，几何解释

1. 尝试

$\begin{bmatrix} x\\y \end{bmatrix} \begin{bmatrix} 1\\0 \end{bmatrix}=x\nRightarrow T(\begin{bmatrix} x\\y \end{bmatrix}) T(\begin{bmatrix} 1\\0 \end{bmatrix})=x\\ \begin{bmatrix} x\\y \end{bmatrix} \begin{bmatrix} 0\\1 \end{bmatrix}=y\nRightarrow T(\begin{bmatrix} x\\y \end{bmatrix}) T(\begin{bmatrix} 0\\1 \end{bmatrix})=y$

**正交变换**： $\forall\vec{v},\vec{w},T(\vec{v})\cdot T(\vec{w})=\vec{v}\cdot\vec{w}$ ，则 $T$ 为**正交变换**（使基向量保持单位长度且相互垂直）

2. 几何转换 克莱姆法则

二维 $SignedArea={\rm det}\pmatrix{ \begin{bmatrix} 0&x\\ 1&y \end{bmatrix}} =1\times y$ （有向面积）

三维 $z={\rm det}\pmatrix{ \begin{bmatrix} 1&0&x\\ 0&1&y\\ 0&0&z \end{bmatrix}}, y={\rm det}\pmatrix{ \begin{bmatrix} 1&x&0\\ 0&y&0\\ 0&z&1 \end{bmatrix}}, x={\rm det}\pmatrix{ \begin{bmatrix} x&0&0\\ y&1&0\\ z&0&1 \end{bmatrix}}$

应用变换后，所有面积伸缩的比例都等于给定的行列式

$y=\frac{Area}{{\rm det}(A)}$

三维及高维也是类似的

## 13 - 计算二阶矩阵特征值的妙计

1）矩阵的迹

$tr={\rm det}\pmatrix{ \begin{bmatrix} a&b\\c&d \end{bmatrix}}=a+d=\lambda_1+\lambda_2$

${\rm mean}(a,d)={\rm mean}(\lambda_1+\lambda_2)$

2）（二阶）矩阵的行列式

$det\pmatrix{ \begin{bmatrix} a&b\\c&d \end{bmatrix}}=ad-bc=\lambda_1\lambda_2$

3）

$\frac{\lambda_1+\lambda_2}{2}=m,\lambda_1\lambda_2=p$ 则 $\lambda_1,\lambda_2=m\pm\sqrt{m^2-p}$
