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

eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%5C%5C-2%20%5Cend%7Bbmatrix%7D%20%3D%203%5Chat%7Bi%7D%2B(-2)%5Chat%7Bj%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%5C%5C-2%20%5Cend%7Bbmatrix%7D%20%3D%203%5Chat%7Bi%7D%2B%28-2%29%5Chat%7Bj%7D&id=l69P3)

**基向量**： ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D%2C%5Chat%7Bj%7D#card=math&code=%5Chat%7Bi%7D%2C%5Chat%7Bj%7D&id=JqyEs) 被称作**基向量**，是**缩放的对象**

![](https://g.yuque.com/gr/latex?a%5Cvec%7Bv%7D%2Bb%5Cvec%7Bw%7D#card=math&code=a%5Cvec%7Bv%7D%2Bb%5Cvec%7Bw%7D&id=zVxOI)

**线性组合**：两个数乘向量的和被称为这两个向量的**线性组合**

![](https://g.yuque.com/gr/latex?%5Cleft%5C%7B%20a%5Cvec%7Bv%7D%2Bb%5Cvec%7Bw%7D%5Cmid%20a%2Cb%5Cin%5Cmathbb%7BR%7D%5Cright%5C%7D#card=math&code=%5Cleft%5C%7B%20a%5Cvec%7Bv%7D%2Bb%5Cvec%7Bw%7D%5Cmid%20a%2Cb%5Cin%5Cmathbb%7BR%7D%5Cright%5C%7D&id=roLsY)

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

![](https://g.yuque.com/gr/latex?%5Cvec%7Bu%7D%5Cne%20a%5Cvec%7Bc%7D%2Bb%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bu%7D%5Cne%20a%5Cvec%7Bc%7D%2Bb%5Cvec%7Bw%7D&id=O83hj)

称它们是**线性无关**的

**向量空间的一组基**（严格定义）：**向量空间的一组基**是张成该空间的一个**线性无关**的向量集

## 03 - 矩阵与线性变换

1.“**变换**” 本质上是 “**函数**” 的一种花哨的说法（向量输入和向量输出）；“**变换**” 暗示用 “**运动**” 的观点思考

2.  **线性变换**：①**任意**直线→直线②原点不变（保持网格线平行且等距分布的变换） 
3.  用数值描述线性变换，考虑 ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D%2C%5Chat%7Bj%7D#card=math&code=%5Chat%7Bi%7D%2C%5Chat%7Bj%7D&id=FdOOe) 的变换，可以确定任意向量的变换；一个二维线性变换仅由四个数字完全确定，即基向量的变换 

4.2×2 矩阵，列理解为两个特殊向量，即变换后的 ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D%2C%5Chat%7Bj%7D#card=math&code=%5Chat%7Bi%7D%2C%5Chat%7Bj%7D&id=UFb0w)

eg. 变换 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%262%5C%5C%20-2%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%262%5C%5C%20-2%261%20%5Cend%7Bbmatrix%7D&id=eKVtB) ，则 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%205%5C%5C%207%20%5Cend%7Bbmatrix%7D%5Crightarrow%205%5Cbegin%7Bbmatrix%7D%203%5C%5C%20-2%20%5Cend%7Bbmatrix%7D%2B%207%5Cbegin%7Bbmatrix%7D%202%5C%5C%201%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%2029%5C%5C%20-3%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%205%5C%5C%207%20%5Cend%7Bbmatrix%7D%5Crightarrow%205%5Cbegin%7Bbmatrix%7D%203%5C%5C%20-2%20%5Cend%7Bbmatrix%7D%2B%207%5Cbegin%7Bbmatrix%7D%202%5C%5C%201%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%2029%5C%5C%20-3%20%5Cend%7Bbmatrix%7D&id=ETYf8)

一般， ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D&id=WX4e1) ，则 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%5Crightarrow%20x%5Cbegin%7Bbmatrix%7D%20a%5C%5C%20c%20%5Cend%7Bbmatrix%7D%2B%20y%5Cbegin%7Bbmatrix%7D%20b%5C%5C%20d%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20ax%2Bby%5C%5C%20cx%2Bdy%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%5Crightarrow%20x%5Cbegin%7Bbmatrix%7D%20a%5C%5C%20c%20%5Cend%7Bbmatrix%7D%2B%20y%5Cbegin%7Bbmatrix%7D%20b%5C%5C%20d%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20ax%2Bby%5C%5C%20cx%2Bdy%20%5Cend%7Bbmatrix%7D&id=jlg9Z)

5. 定义矩阵乘法

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%3D%20x%5Cbegin%7Bbmatrix%7D%20a%5C%5C%20c%20%5Cend%7Bbmatrix%7D%2B%20y%5Cbegin%7Bbmatrix%7D%20b%5C%5C%20d%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20ax%2Bby%5C%5C%20cx%2Bdy%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%3D%20x%5Cbegin%7Bbmatrix%7D%20a%5C%5C%20c%20%5Cend%7Bbmatrix%7D%2B%20y%5Cbegin%7Bbmatrix%7D%20b%5C%5C%20d%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20ax%2Bby%5C%5C%20cx%2Bdy%20%5Cend%7Bbmatrix%7D&id=fzp9J)

## 04 - 矩阵乘法与线性变换复合

1. **旋转**与**剪切**的 “复合变换”

eg.

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D%20%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%200%261%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D%20%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%200%261%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5C%20y%20%5Cend%7Bbmatrix%7D&id=SWSPE)

其中 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D&id=VpRph) 为旋转矩阵，![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D&id=SVfKd) 为剪切矩阵， ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D&id=A7DgV) 为复合矩阵

![](https://g.yuque.com/gr/latex?%5Ctherefore%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D#card=math&code=%5Ctherefore%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%201%260%20%5Cend%7Bbmatrix%7D&id=KKHpU)

两个矩阵相乘有着几何意义，也就是**两个线性变换相继作用**

2. 矩阵的乘法

eg.

![](https://g.yuque.com/gr/latex?M_1%3D%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%2C%20M_2%3D%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%2C%20M_2%20M_1%3D%20%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%3F#card=math&code=M_1%3D%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%2C%20M_2%3D%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%2C%20M_2%20M_1%3D%20%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%3F&id=QfKHp)

Where does ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D#card=math&code=%5Chat%7Bi%7D&id=wtkzW) go?

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%5C%5C%201%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%5C%5C%201%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%5C%5C%201%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%5C%5C%201%20%5Cend%7Bbmatrix%7D&id=vF5vd)

类似地， ![](https://g.yuque.com/gr/latex?%5Chat%7Bj%7D#card=math&code=%5Chat%7Bj%7D&id=GvyHO)

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20-2%5C%5C%200%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C%20-2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20-2%5C%5C%200%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C%20-2%20%5Cend%7Bbmatrix%7D&id=syo3p)

![](https://g.yuque.com/gr/latex?%5Ctherefore%20M_2%20M_1%3D%20%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%260%5C%5C%201%26-2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Ctherefore%20M_2%20M_1%3D%20%5Cbegin%7Bbmatrix%7D%200%262%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-2%5C%5C%201%260%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%260%5C%5C%201%26-2%20%5Cend%7Bbmatrix%7D&id=WRO14)

一般，

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20e%26f%5C%5C%20g%26h%20%5Cend%7Bbmatrix%7D%20%3D%20%5Cbegin%7Bbmatrix%7D%20ae%2Bbg%26af%2Bbh%5C%5C%20ce%2Bdg%26cf%2Bdh%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20e%26f%5C%5C%20g%26h%20%5Cend%7Bbmatrix%7D%20%3D%20%5Cbegin%7Bbmatrix%7D%20ae%2Bbg%26af%2Bbh%5C%5C%20ce%2Bdg%26cf%2Bdh%20%5Cend%7Bbmatrix%7D&id=iUHHu)

3. **矩阵乘法交换律不成立**

![](https://g.yuque.com/gr/latex?M_1%20M_2%5Cne%20M_2%20M_1#card=math&code=M_1%20M_2%5Cne%20M_2%20M_1&id=YlMPl)

4. **矩阵乘法结合律成立**

![](https://g.yuque.com/gr/latex?(AB)C%3DA(BC)#card=math&code=%28AB%29C%3DA%28BC%29&id=nXqnn)

## 附注 1 - 三维空间中的线性变换

## 05 - 行列式

1. 行列式

**行列式**：线性变换**改变面积的比例**（由于网格线平行等距，对任意图形缩放比例相等）被称为这个变换的**行列式**

eg. ![](https://g.yuque.com/gr/latex?%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%203%262%5C%5C%200%262%20%5Cend%7Bbmatrix%7D%7D%3D6#card=math&code=%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%203%262%5C%5C%200%262%20%5Cend%7Bbmatrix%7D%7D%3D6&id=f0rd8)

2.  行列式的正负与平面的取向有关；行列式为负，空间被翻转；三维翻转，右手系变为左手系 
3.  行列式的计算 

![](https://g.yuque.com/gr/latex?%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%7D%20%3Dad-bc#card=math&code=%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5C%20c%26d%20%5Cend%7Bbmatrix%7D%7D%20%3Dad-bc&id=ndI1u)

![](https://pic4.zhimg.com/v2-73f5933ea50afddc59797a1369faaaf7_r.jpg#crop=0&crop=0&crop=1&crop=1&id=HExKh&originHeight=340&originWidth=720&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

![](https://g.yuque.com/gr/latex?%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20a%26b%26c%5C%5C%20d%26e%26f%5C%5C%20g%26h%26i%20%5Cend%7Bbmatrix%7D%7D%3D%20a%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20e%26f%5C%5C%20h%26i%20%5Cend%7Bbmatrix%7D%7D%20-b%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20d%26f%5C%5C%20g%26i%20%5Cend%7Bbmatrix%7D%7D%20%2Bc%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20d%26e%5C%5C%20g%26h%20%5Cend%7Bbmatrix%7D%7D#card=math&code=%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20a%26b%26c%5C%5C%20d%26e%26f%5C%5C%20g%26h%26i%20%5Cend%7Bbmatrix%7D%7D%3D%20a%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20e%26f%5C%5C%20h%26i%20%5Cend%7Bbmatrix%7D%7D%20-b%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20d%26f%5C%5C%20g%26i%20%5Cend%7Bbmatrix%7D%7D%20%2Bc%5C%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20d%26e%5C%5C%20g%26h%20%5Cend%7Bbmatrix%7D%7D&id=dgrRB)

## 06 - 逆矩阵、列空间与零空间

1. 线性方程组与向量方程

eg.

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%202x%2B5y%2B3z%3D-3%5C%5C%204x%2B0y%2B8z%3D0%5C%5C%201x%2B3y%2B0z%3D2%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D%5Crightarrow%20%5Cbegin%7Bbmatrix%7D%202%265%263%5C%5C%204%260%268%5C%5C%201%263%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-3%5C%5C0%5C%5C2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%202x%2B5y%2B3z%3D-3%5C%5C%204x%2B0y%2B8z%3D0%5C%5C%201x%2B3y%2B0z%3D2%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D%5Crightarrow%20%5Cbegin%7Bbmatrix%7D%202%265%263%5C%5C%204%260%268%5C%5C%201%263%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-3%5C%5C0%5C%5C2%20%5Cend%7Bbmatrix%7D&id=LCENi)

![](https://g.yuque.com/gr/latex?A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D&id=vG5SD) 其中 ![](https://g.yuque.com/gr/latex?A#card=math&code=A&id=FzWG5) 为系数矩阵， ![](https://g.yuque.com/gr/latex?%5Cvec%7Bx%7D#card=math&code=%5Cvec%7Bx%7D&id=KL4uJ) 为包含未知数的向量， ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=Gcvcx) 为常数向量

2. 几何解释

![](https://g.yuque.com/gr/latex?A#card=math&code=A&id=vcCyX) 代表一种线性变换，向量方程意义是找到 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bx%7D#card=math&code=%5Cvec%7Bx%7D&id=dFR06) 经过变换后与 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=If67H) 重合

3. 方程求解

当 ![](https://g.yuque.com/gr/latex?%7B%5Crm%20det%7D(A)%5Cne0#card=math&code=%7B%5Crm%20det%7D%28A%29%5Cne0&id=lFt4C) ， ![](https://g.yuque.com/gr/latex?%5Cvec%7Bx%7D%2C%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bx%7D%2C%5Cvec%7Bv%7D&id=JiIqg) 一一对应； ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=j6ULB) 经过逆变换得 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bx%7D#card=math&code=%5Cvec%7Bx%7D&id=E46fb)

![](https://g.yuque.com/gr/latex?A#card=math&code=A&id=i37on) 的逆记为 ![](https://g.yuque.com/gr/latex?A%5E%7B-1%7D#card=math&code=A%5E%7B-1%7D&id=CBGI9)

![](https://g.yuque.com/gr/latex?A%5E%7B-1%7DA%3D%20%5Cbegin%7Bbmatrix%7D%201%260%5C%5C%200%261%20%5Cend%7Bbmatrix%7D#card=math&code=A%5E%7B-1%7DA%3D%20%5Cbegin%7Bbmatrix%7D%201%260%5C%5C%200%261%20%5Cend%7Bbmatrix%7D&id=bBGUh)

![](https://g.yuque.com/gr/latex?A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D%5C%5C%20A%5E%7B-1%7DA%5Cvec%7Bx%7D%3DA%5E%7B-1%7D%5Cvec%7Bv%7D%5C%5C%20%5Ctherefore%20%5Cvec%7Bx%7D%3DA%5E%7B-1%7D%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D%5C%5C%20A%5E%7B-1%7DA%5Cvec%7Bx%7D%3DA%5E%7B-1%7D%5Cvec%7Bv%7D%5C%5C%20%5Ctherefore%20%5Cvec%7Bx%7D%3DA%5E%7B-1%7D%5Cvec%7Bv%7D&id=lwWd8)

当 ![](https://g.yuque.com/gr/latex?det(A)%3D0#card=math&code=det%28A%29%3D0&id=NSHk4) ，没有逆变换（不能 “解压缩”）；**可能有解**

4. 列空间

**列空间**：所有可能的输出向量 ![](https://g.yuque.com/gr/latex?A%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bv%7D&id=aEiXW) 构成的集合被称为 ![](https://g.yuque.com/gr/latex?A#card=math&code=A&id=gly31) 的**列空间**

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

对线性方程组 ![](https://g.yuque.com/gr/latex?A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bx%7D%3D%5Cvec%7Bv%7D&id=JUlpd) ，当 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C0%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cvec%7Bv%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C0%20%5Cend%7Bbmatrix%7D&id=DpZO6) 时，零空间给出的就是这个向量方程的**所有解**

7. 总结

以上就是从集合角度理解线性方程组的一个高水平概述

每个方程组都有一个线性变换与之联系

当逆变换存在时，可用逆变换求解方程组

否则，列空间的概念让我们清楚什么时候存在解

零空间的概念有助于理解所有可能的解的集合是什么样的

## 附注 2 - 非方阵

1. 非方阵的几何含义

eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%260%5C%5C%20-1%261%5C%5C%20-2%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%260%5C%5C%20-1%261%5C%5C%20-2%261%20%5Cend%7Bbmatrix%7D&id=H0Z2u) 这个变换将 ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D#card=math&code=%5Chat%7Bi%7D&id=FHIt4) 变换到坐标 ![](https://g.yuque.com/gr/latex?(2%2C-1%2C-2)#card=math&code=%282%2C-1%2C-2%29&id=eeTnq) ， ![](https://g.yuque.com/gr/latex?%5Chat%7Bj%7D#card=math&code=%5Chat%7Bj%7D&id=jMqR6) 变换到坐标 ![](https://g.yuque.com/gr/latex?(0%2C1%2C1)#card=math&code=%280%2C1%2C1%29&id=l0WXr)

![](https://pic2.zhimg.com/v2-1e340b1a02f5d982530ff278367f7c2d_r.jpg#crop=0&crop=0&crop=1&crop=1&id=Utteq&originHeight=389&originWidth=680&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

这个变换是**满秩**的；是二维向三维的映射

## 07 - 点积与对偶性

> 卡尔文：你知道吗，我觉得数学不是一门科学，而是一种宗教。
霍布斯：一种宗教？
卡尔文：是啊。这些公式就像奇迹一般。你取出两个数，把它们相加时，他们神奇地成为了一个全新的数！没人能说清这到底是怎么发生的。你要么完全相信，要么完全不信。


1. 标准观点

eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%5C%5C2%20%5Cend%7Bbmatrix%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%203%5C%5C4%20%5Cend%7Bbmatrix%7D%3D%201%5Ccdot3%2B2%5Ccdot4#card=math&code=%5Cbegin%7Bbmatrix%7D%201%5C%5C2%20%5Cend%7Bbmatrix%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%203%5C%5C4%20%5Cend%7Bbmatrix%7D%3D%201%5Ccdot3%2B2%5Ccdot4&id=n15V9)

![](https://pic1.zhimg.com/v2-1535a06c4964fbf911eeaa2e81fd2cb8_r.jpg#crop=0&crop=0&crop=1&crop=1&id=XkFvW&originHeight=403&originWidth=685&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

2. 为什么点积与顺序无关

如果 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=p5myZ) 的长度恰好相同，可以利用**对称性**（ ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=HTWqs) 向 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=Efhtw) 上的投影等于 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=xw0XL) 向 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=GQ2eo) 上的投影）

如果它们的长度不同，例如 ![](https://g.yuque.com/gr/latex?2%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=2%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=dP1Yq)

当 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=HD2eO) 向 ![](https://g.yuque.com/gr/latex?2%5Cvec%7Bv%7D#card=math&code=2%5Cvec%7Bv%7D&id=qswL7) 上投影， ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=Oe8G1) 的投影长度不变，![](https://g.yuque.com/gr/latex?(2%5Cvec%7Bv%7D)%5Ccdot%5Cvec%7Bw%7D%3D2(%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D)#card=math&code=%282%5Cvec%7Bv%7D%29%5Ccdot%5Cvec%7Bw%7D%3D2%28%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D%29&id=fRir4)

当 ![](https://g.yuque.com/gr/latex?2%5Cvec%7Bv%7D#card=math&code=2%5Cvec%7Bv%7D&id=pvDd7) 向 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=kYiMO) 上投影， ![](https://g.yuque.com/gr/latex?2%5Cvec%7Bv%7D#card=math&code=2%5Cvec%7Bv%7D&id=sVw19) 的投影长度变为两倍，![](https://g.yuque.com/gr/latex?(2%5Cvec%7Bv%7D)%5Ccdot%5Cvec%7Bw%7D%3D2(%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D)#card=math&code=%282%5Cvec%7Bv%7D%29%5Ccdot%5Cvec%7Bw%7D%3D2%28%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D%29&id=T7YIi)

即使对称性被破坏，两种理解下，缩放向量对点积结果的影响是相同的

3. 点积和投影的联系：**对偶性**

多维空间到一维空间（数轴）的线性变换

eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-2%20%5Cend%7Bbmatrix%7D%5Cbegin%7Bbmatrix%7D%204%5C%5C3%20%5Cend%7Bbmatrix%7D%3D%204%5Ccdot1%2B3%5Ccdot(-2)#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-2%20%5Cend%7Bbmatrix%7D%5Cbegin%7Bbmatrix%7D%204%5C%5C3%20%5Cend%7Bbmatrix%7D%3D%204%5Ccdot1%2B3%5Ccdot%28-2%29&id=vU0Xo)

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-2%20%5Cend%7Bbmatrix%7D&id=cspuc) 为变换（看作**倾倒的向量**）， ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%204%5C%5C3%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%204%5C%5C3%20%5Cend%7Bbmatrix%7D&id=v3oJH) 为向量

设一数轴的单位向量为 ![](https://g.yuque.com/gr/latex?%5Chat%7Bu%7D#card=math&code=%5Chat%7Bu%7D&id=qN8w1)

![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D#card=math&code=%5Chat%7Bi%7D&id=onyW0) 向 ![](https://g.yuque.com/gr/latex?%5Chat%7Bu%7D#card=math&code=%5Chat%7Bu%7D&id=tfRYy) 所在直线的投影与 ![](https://g.yuque.com/gr/latex?%5Chat%7Bu%7D#card=math&code=%5Chat%7Bu%7D&id=wP3Fv) 向 ![](https://g.yuque.com/gr/latex?x#card=math&code=x&id=pzmim) 轴投影**完全对称**

对 ![](https://g.yuque.com/gr/latex?%5Chat%7Bj%7D#card=math&code=%5Chat%7Bj%7D&id=RnGOC) 同理

![](https://g.yuque.com/gr/latex?%5Ctherefore#card=math&code=%5Ctherefore&id=hJ9dI) 二维空间向该数轴的线性变换为 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20u_x%26u_y%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20u_x%26u_y%20%5Cend%7Bbmatrix%7D&id=oGUUH)

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20u_x%26u_y%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%3D%20u_x%5Ccdot%20x%2Bu_y%5Ccdot%20y#card=math&code=%5Cbegin%7Bbmatrix%7D%20u_x%26u_y%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%3D%20u_x%5Ccdot%20x%2Bu_y%5Ccdot%20y&id=Wd010) （矩阵向量乘积）

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20u_x%5C%5Cu_y%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%3D%20u_x%5Ccdot%20x%2Bu_y%5Ccdot%20y#card=math&code=%5Cbegin%7Bbmatrix%7D%20u_x%5C%5Cu_y%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%3D%20u_x%5Ccdot%20x%2Bu_y%5Ccdot%20y&id=tzvIo) （点积）

若 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bu%7D#card=math&code=%5Cvec%7Bu%7D&id=blfCa) 为非单位向量，结合对称性被破坏时的**顺序无关**，同理可得

## 08 第一部分 - 叉积的标准介绍

1. 二维叉积

![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D&id=RJQpV) **数值**为它们所张成的**平行四边形的面积**，“**正负**” 由**右手定则**决定；用**行列式**计算

eg. ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-3%5C%5C1%20%5Cend%7Bbmatrix%7D%20%2C%5Cvec%7Bw%7D%20%3D%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cvec%7Bv%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-3%5C%5C1%20%5Cend%7Bbmatrix%7D%20%2C%5Cvec%7Bw%7D%20%3D%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D&id=YA0EU)

![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%203%262%5C%5C1%261%20%5Cend%7Bbmatrix%7D%7D%20%3D-3%5Ccdot1-2%5Ccdot1%3D-5#card=math&code=%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%203%262%5C%5C1%261%20%5Cend%7Bbmatrix%7D%7D%20%3D-3%5Ccdot1-2%5Ccdot1%3D-5&id=ScYED)

两个向量所成平行四边形的面积为 5，且因为 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=c8h3n) 在 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bw%7D&id=sHsPi) 的左侧，结果为负

此外，![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=rMbrI) 越接近垂直，面积越大； ![](https://g.yuque.com/gr/latex?(a%5Cvec%7Bv%7D)%5Ctimes%5Cvec%7Bw%7D%3Da(%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D)#card=math&code=%28a%5Cvec%7Bv%7D%29%5Ctimes%5Cvec%7Bw%7D%3Da%28%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D%29&id=XRFa4)

2. 真正的叉积

真正的叉积是通过两个三维向量生成一个新的三维向量

![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D%3D%5Cvec%7Bp%7D#card=math&code=%5Cvec%7Bv%7D%5Ctimes%5Cvec%7Bw%7D%3D%5Cvec%7Bp%7D&id=ke5Ui)

![](https://g.yuque.com/gr/latex?%5Cvec%7Bp%7D#card=math&code=%5Cvec%7Bp%7D&id=YkxPD) 长度为平行四边形的面积，方向于平行四边形所在的面垂直，遵循右手定则

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20v_1%5C%5Cv_2%5C%5Cv_3%20%5Cend%7Bbmatrix%7D%5Ctimes%20%5Cbegin%7Bbmatrix%7D%20w_1%5C%5Cw_2%5C%5Cw_3%20%5Cend%7Bbmatrix%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20%5Chat%7Bi%7D%26v_1%26w_1%5C%5C%20%5Chat%7Bj%7D%26v_2%26w_2%5C%5C%20%5Chat%7Bk%7D%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20v_1%5C%5Cv_2%5C%5Cv_3%20%5Cend%7Bbmatrix%7D%5Ctimes%20%5Cbegin%7Bbmatrix%7D%20w_1%5C%5Cw_2%5C%5Cw_3%20%5Cend%7Bbmatrix%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20%5Chat%7Bi%7D%26v_1%26w_1%5C%5C%20%5Chat%7Bj%7D%26v_2%26w_2%5C%5C%20%5Chat%7Bk%7D%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D&id=NpUKp)

## 08 第二部分 - 以线性变换的眼光看叉积

1. 回顾

**对偶性**的思想在于，一个空间到数轴的线性变换与空间中唯一一个向量对应，也就是说**应用线性变换与向量点乘等价**

这样的向量被称为这个变换的**对偶向量**

2. 三维空间到数轴的特定线性变换

![](https://g.yuque.com/gr/latex?f%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%26v_1%26w_1%5C%5C%20y%26v_2%26w_2%5C%5C%20z%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D#card=math&code=f%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%26v_1%26w_1%5C%5C%20y%26v_2%26w_2%5C%5C%20z%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D&id=O1W6p)

这个函数的几何意义是，对于任一输入的向量 ![](https://g.yuque.com/gr/latex?(x%2Cy%2Cz)#card=math&code=%28x%2Cy%2Cz%29&id=QmW9L) ，输出由它和 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=nyPxn) 确定的**平行六面体体积**（有正负）

这个函数是**线性的**，因而可以写成矩阵乘法

又因为应用这个变换和与对偶向量点乘等价，所以

![](https://g.yuque.com/gr/latex?%5Cvec%7Bp%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20p_1%5C%5Cp_2%5C%5Cp_3%20%5Cend%7Bbmatrix%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%26v_1%26w_1%5C%5C%20y%26v_2%26w_2%5C%5C%20z%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D#card=math&code=%5Cvec%7Bp%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20p_1%5C%5Cp_2%5C%5Cp_3%20%5Cend%7Bbmatrix%7D%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D%3D%20%7B%5Crm%20det%7D%5Cpmatrix%7B%5Cbegin%7Bbmatrix%7D%20x%26v_1%26w_1%5C%5C%20y%26v_2%26w_2%5C%5C%20z%26v_3%26w_3%20%5Cend%7Bbmatrix%7D%7D&id=SUh6M)

![](https://g.yuque.com/gr/latex?p_1%5Ccdot%20x%2Bp_2%5Ccdot%20y%2Bp_3%5Ccdot%20z%3D%20x(v_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2)%2B%20y(v_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3)%2B%20z(v_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1)#card=math&code=p_1%5Ccdot%20x%2Bp_2%5Ccdot%20y%2Bp_3%5Ccdot%20z%3D%20x%28v_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2%29%2B%20y%28v_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3%29%2B%20z%28v_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1%29&id=XZqNq)

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%20p_1%3Dv_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2%5C%5C%20p_2%3Dv_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3%5C%5C%20p_3%3Dv_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D#card=math&code=%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%20p_1%3Dv_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2%5C%5C%20p_2%3Dv_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3%5C%5C%20p_3%3Dv_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D&id=j3OfJ)

比较 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20v_1%5C%5Cv_2%5C%5Cv_3%20%5Cend%7Bbmatrix%7D%5Ctimes%20%5Cbegin%7Bbmatrix%7D%20w_1%5C%5Cw_2%5C%5Cw_3%20%5Cend%7Bbmatrix%7D%3D%20%5Chat%7Bi%7D(v_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2)%2B%20%5Chat%7Bj%7D(v_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3)%2B%20%5Chat%7Bk%7D(v_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1)#card=math&code=%5Cbegin%7Bbmatrix%7D%20v_1%5C%5Cv_2%5C%5Cv_3%20%5Cend%7Bbmatrix%7D%5Ctimes%20%5Cbegin%7Bbmatrix%7D%20w_1%5C%5Cw_2%5C%5Cw_3%20%5Cend%7Bbmatrix%7D%3D%20%5Chat%7Bi%7D%28v_2%5Ccdot%20w_3-v_3%5Ccdot%20w_2%29%2B%20%5Chat%7Bj%7D%28v_3%5Ccdot%20w_1-v_1%5Ccdot%20w_3%29%2B%20%5Chat%7Bk%7D%28v_1%5Ccdot%20w_2-v_2%5Ccdot%20w_1%29&id=oxcnY)

3. 什么样的 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bp%7D#card=math&code=%5Cvec%7Bp%7D&id=O4X18) 满足条件

![](https://g.yuque.com/gr/latex?p%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D#card=math&code=p%5Ccdot%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%5C%5Cz%20%5Cend%7Bbmatrix%7D&id=LGLjk) 的几何解释是把其他向量向 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bp%7D#card=math&code=%5Cvec%7Bp%7D&id=kapkH) 投影的长度与 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bp%7D#card=math&code=%5Cvec%7Bp%7D&id=tsEg2) 的长度相乘

平行六面体的体积

= 平行四边形的面积乘 ![](https://g.yuque.com/gr/latex?(x%2Cy%2Cz)#card=math&code=%28x%2Cy%2Cz%29&id=QLG0A) 垂直于 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=fGsMf) 的分量

= 垂直于 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=wLXG0) 且长度为平行四边形面积的向量与 ![](https://g.yuque.com/gr/latex?(x%2Cy%2Cz)#card=math&code=%28x%2Cy%2Cz%29&id=Y988q) 点乘

点积为正的情况会与 ![](https://g.yuque.com/gr/latex?(x%2Cy%2Cz)%2C%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%28x%2Cy%2Cz%29%2C%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=WPZRS) 满足右手定则的情况吻合

这就是**叉积的计算**与**几何解释**有关联的根本原因

3. 总结

首先，定义一个三维空间到数轴的线性变换

然后，考虑这个变换的对偶向量

①应用这个变换和与对偶向量点乘等价

②从几何角度思考，这个对偶向量必然与 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D#card=math&code=%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D&id=yDwSI) 垂直，长度等于两个向量张成的平四面积

## 09 - 基变换

1. 坐标系和基向量

**坐标系**：发生在向量与一组数之间的任意一种转化，都被称为一个**坐标系**

其中两个特殊的向量 ![](https://g.yuque.com/gr/latex?%5Chat%7Bi%7D%2C%5Chat%7Bj%7D#card=math&code=%5Chat%7Bi%7D%2C%5Chat%7Bj%7D&id=PA9Qs) 被称为这个坐标系的**基向量**

2. 讨论使用另一组基向量的思想

将基向量理解为 “**语言**”

**如何在不同坐标系之间转化？**

eg. 我看 Jenny 的基向量 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bb_1%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D%20%5Cvec%7Bb_2%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cvec%7Bb_1%7D%3D%20%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D%20%5Cvec%7Bb_2%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D&id=fR9H5)

对于同一个向量，我看是 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%5C%5C2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%5C%5C2%20%5Cend%7Bbmatrix%7D&id=Ir0FZ) ，Jenny 看是  ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B5%7D%7B3%7D%5C%5C%5Cfrac%7B1%7D%7B3%7D%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B5%7D%7B3%7D%5C%5C%5Cfrac%7B1%7D%7B3%7D%20%5Cend%7Bbmatrix%7D&id=oiOvz) （不同的语言描述同一个向量）

Jenny 用 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20-1%5C%5C2%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20-1%5C%5C2%20%5Cend%7Bbmatrix%7D&id=IJJEx) 表示一个向量，在我们的坐标系如何描述？（如何从她的语言转化到我们的语言？）

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20-1%5C%5C2%20%5Cend%7Bbmatrix%7D%3D%20-1%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D%2B%202%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-4%5C%5C1%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20-1%5C%5C2%20%5Cend%7Bbmatrix%7D%3D%20-1%5Cbegin%7Bbmatrix%7D%202%5C%5C1%20%5Cend%7Bbmatrix%7D%2B%202%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20-4%5C%5C1%20%5Cend%7Bbmatrix%7D&id=bQ29D)

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C%201%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C%201%261%20%5Cend%7Bbmatrix%7D&id=g9qpt) 从几何上，将我们的网格变换为 Jenny 的网格；从数值上，将她的语言转化为我们的语言（相反的）

把它看作我们对 Jenny 的向量的误解，也就是我们的坐标系有相同坐标的向量，变换成真正想表示的向量

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D&id=fyVfv) 将 Jenny 的网格变换为我们的网格；将我们的语言转化为她的语言

Jenny 如何描述同样的空间 ![](https://g.yuque.com/gr/latex?90%5E%7B%5Ccirc%7D#card=math&code=90%5E%7B%5Ccirc%7D&id=jHH9P) 旋转？

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D&id=r7zrb) 转化成我们的语言

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C1%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C1%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D&id=uq6GA) 用我们的语言描述变换矩阵

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C1%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%200%26-1%5C%5C1%260%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%202%26-1%5C%5C1%261%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D&id=Y5Vxq) 用她的语言描述变换后的向量

表达式 ![](https://g.yuque.com/gr/latex?A%5E%7B-1%7DMA#card=math&code=A%5E%7B-1%7DMA&id=Ohncp) 暗示着一种数学上的**转移作用**，中间的矩阵代表**你所见的变换**

## 10 - 特征向量与特征值

1. 特征向量与特征值

满足 ![](https://g.yuque.com/gr/latex?A%5Cvec%7Bv%7D%3D%5Clambda%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bv%7D%3D%5Clambda%5Cvec%7Bv%7D&id=UsRnW)

将等号右侧重写为某个矩阵向量乘积

![](https://g.yuque.com/gr/latex?%5Clambda%5Cvec%7Bv%7D#card=math&code=%5Clambda%5Cvec%7Bv%7D&id=FGvix) 表示 ![](https://g.yuque.com/gr/latex?%5Cvec%7Bv%7D#card=math&code=%5Cvec%7Bv%7D&id=A8qSk) 的每个基向量与 ![](https://g.yuque.com/gr/latex?%5Clambda#card=math&code=%5Clambda&id=Yp3gs) 相乘，因此可以重写为 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20%5Clambda%260%260%5C%5C%200%26%5Clambda%260%5C%5C%200%260%26%5Clambda%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20%5Clambda%260%260%5C%5C%200%26%5Clambda%260%5C%5C%200%260%26%5Clambda%20%5Cend%7Bbmatrix%7D%5Cvec%7Bv%7D&id=Cyarp)

![](https://g.yuque.com/gr/latex?A%5Cvec%7Bv%7D%3D(%5Clambda%20I)%5Cvec%7Bv%7D#card=math&code=A%5Cvec%7Bv%7D%3D%28%5Clambda%20I%29%5Cvec%7Bv%7D&id=zMw89)

![](https://g.yuque.com/gr/latex?(A-%5Clambda%20I)%5Cvec%7Bv%7D%3D%5Cvec%7B0%7D#card=math&code=%28A-%5Clambda%20I%29%5Cvec%7Bv%7D%3D%5Cvec%7B0%7D&id=O8j5c)

当且仅当矩阵代表的变换将空间**压缩到更低维度**时，才会存在满足上式的非零向量

![](https://g.yuque.com/gr/latex?%5Ctherefore%20%7B%5Crm%20det%7D(A-%5Clambda%20I)%3D0#card=math&code=%5Ctherefore%20%7B%5Crm%20det%7D%28A-%5Clambda%20I%29%3D0&id=UJnaF)

二维线性变换不一定有特征向量，如旋转 90 度的变换

2. 特征基与对角化

如果基向量都是特征向量，eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20-1%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%20-1%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D&id=sUc76)

**对角矩阵**：除了对角元以外其他元素均为 0 的矩阵被称为**对角矩阵**

对角矩阵所有的基向量都是特征向量，矩阵的**对角元**是它们**所属的特征值**

用特征向量作为基

eg. ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D&id=UnztD) 取特征向量 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D%20%2C%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D%20%2C%5Cbegin%7Bbmatrix%7D%20-1%5C%5C1%20%5Cend%7Bbmatrix%7D&id=FJrVX) 作为基

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D&id=D1BRf) 新矩阵必然是对角的

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D&id=M2ZbG)

**特征基**：一组特征向量作为基向量构成的集合被称为一组**特征基**

计算 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D&id=Vo1g6) ，一种更容易的做法是先变换到特征基，计算 100 次幂，然后转化回标准系

> 解：
计算特征值和特征向量，得特征基变换矩阵 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%200%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C%200%261%20%5Cend%7Bbmatrix%7D&id=zKFJi) ，并求出它的逆 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C%200%261%20%5Cend%7Bbmatrix%7D&id=i0Mqx)
对角化， ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%20%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D&id=brR60)
特征基下， ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%260%5C%5C%200%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%260%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%260%5C%5C%200%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D&id=yuRdd)
回到标准系，得 ![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%260%5C%5C0%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%263%5E%7B100%7D-2%5E%7B100%7D%5C%5C0%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cbegin%7Bbmatrix%7D%203%261%5C%5C0%262%20%5Cend%7Bbmatrix%7D%5E%7B100%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%260%5C%5C0%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%26-1%5C%5C0%261%20%5Cend%7Bbmatrix%7D%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%203%5E%7B100%7D%263%5E%7B100%7D-2%5E%7B100%7D%5C%5C0%262%5E%7B100%7D%20%5Cend%7Bbmatrix%7D&id=iIBDZ)


并非所有矩阵都能对角化，如剪切矩阵（特征向量不能张成全空间）

![](https://pic4.zhimg.com/v2-71f972bec56e09362f002eca4bab950b_r.jpg#crop=0&crop=0&crop=1&crop=1&id=nrYSz&originHeight=435&originWidth=727&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

> 解：
![](https://g.yuque.com/gr/latex?A%5E2%3D%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C1%262%20%5Cend%7Bbmatrix%7D%2C%20A%5E3%3D%5Cbegin%7Bbmatrix%7D%201%262%5C%5C2%263%20%5Cend%7Bbmatrix%7D%2C%20A%5E4%3D%5Cbegin%7Bbmatrix%7D%202%263%5C%5C3%265%20%5Cend%7Bbmatrix%7D%2C%20A%5E5%3D%5Cbegin%7Bbmatrix%7D%203%265%5C%5C5%268%20%5Cend%7Bbmatrix%7D#card=math&code=A%5E2%3D%20%5Cbegin%7Bbmatrix%7D%201%261%5C%5C1%262%20%5Cend%7Bbmatrix%7D%2C%20A%5E3%3D%5Cbegin%7Bbmatrix%7D%201%262%5C%5C2%263%20%5Cend%7Bbmatrix%7D%2C%20A%5E4%3D%5Cbegin%7Bbmatrix%7D%202%263%5C%5C3%265%20%5Cend%7Bbmatrix%7D%2C%20A%5E5%3D%5Cbegin%7Bbmatrix%7D%203%265%5C%5C5%268%20%5Cend%7Bbmatrix%7D&id=eNCXS)
猜想 ![](https://g.yuque.com/gr/latex?A%5En%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn-1%7D%26F_n%5C%5CF_%7Bn%7D%26F_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D#card=math&code=A%5En%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn-1%7D%26F_n%5C%5CF_%7Bn%7D%26F_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D&id=kDjYm) ，其中 ![](https://g.yuque.com/gr/latex?%5C%7BF_n%5C%7D#card=math&code=%5C%7BF_n%5C%7D&id=mLNaZ) 为斐波那契数列
证明（数学归纳法）：
![](https://g.yuque.com/gr/latex?n%3D1#card=math&code=n%3D1&id=dNYVl) 时，猜想成立；
若 ![](https://g.yuque.com/gr/latex?n%3Dk#card=math&code=n%3Dk&id=EwG8p) 时成立，则
![](https://g.yuque.com/gr/latex?A%5E%7Bk%2B1%7D%3D%5Cbegin%7Bbmatrix%7D%200%261%5C%5C1%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn-1%7D%26F_n%5C%5CF_%7Bn%7D%26F_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn%7D%26F_%7Bn%2B1%7D%5C%5CF_%7Bn-1%7D%2BF_%7Bn%7D%26F_%7Bn%7D%2BF_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn%7D%26F_%7Bn%2B1%7D%5C%5CF_%7Bn%2B1%7D%26F_%7Bn%2B2%7D%20%5Cend%7Bbmatrix%7D#card=math&code=A%5E%7Bk%2B1%7D%3D%5Cbegin%7Bbmatrix%7D%200%261%5C%5C1%261%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn-1%7D%26F_n%5C%5CF_%7Bn%7D%26F_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn%7D%26F_%7Bn%2B1%7D%5C%5CF_%7Bn-1%7D%2BF_%7Bn%7D%26F_%7Bn%7D%2BF_%7Bn%2B1%7D%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%20F_%7Bn%7D%26F_%7Bn%2B1%7D%5C%5CF_%7Bn%2B1%7D%26F_%7Bn%2B2%7D%20%5Cend%7Bbmatrix%7D&id=nnFmF)
符合猜想
QED
解法（特征基）：
特征基变换矩阵 ![](https://g.yuque.com/gr/latex?M%3D%5Cbegin%7Bbmatrix%7D%202%262%5C%5C1%2B%5Csqrt%7B5%7D%261-%5Csqrt%7B5%7D%20%5Cend%7Bbmatrix%7D#card=math&code=M%3D%5Cbegin%7Bbmatrix%7D%202%262%5C%5C1%2B%5Csqrt%7B5%7D%261-%5Csqrt%7B5%7D%20%5Cend%7Bbmatrix%7D&id=NLUTE) ，求出它的逆 ![](https://g.yuque.com/gr/latex?M%5E%7B-1%3D%7D%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B5-%5Csqrt%7B5%7D%7D%7B20%7D%26%5Cfrac%7B%5Csqrt%7B5%7D%7D%7B10%7D%5C%5C%20%5Cfrac%7B5%2B%5Csqrt%7B5%7D%7D%7B20%7D%26-%5Cfrac%7B%5Csqrt%7B5%7D%7D%7B10%7D%20%5Cend%7Bbmatrix%7D#card=math&code=M%5E%7B-1%3D%7D%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B5-%5Csqrt%7B5%7D%7D%7B20%7D%26%5Cfrac%7B%5Csqrt%7B5%7D%7D%7B10%7D%5C%5C%20%5Cfrac%7B5%2B%5Csqrt%7B5%7D%7D%7B20%7D%26-%5Cfrac%7B%5Csqrt%7B5%7D%7D%7B10%7D%20%5Cend%7Bbmatrix%7D&id=GRHih)
对角化， ![](https://g.yuque.com/gr/latex?M%5E%7B-1%7DAM%3D%20%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B1%2B%5Csqrt%7B5%7D%7D%7B2%7D%260%5C%5C%200%26%5Cfrac%7B1-%5Csqrt%7B5%7D%7D%7B2%7D%20%5Cend%7Bbmatrix%7D#card=math&code=M%5E%7B-1%7DAM%3D%20%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B1%2B%5Csqrt%7B5%7D%7D%7B2%7D%260%5C%5C%200%26%5Cfrac%7B1-%5Csqrt%7B5%7D%7D%7B2%7D%20%5Cend%7Bbmatrix%7D&id=rogk1)
![](https://g.yuque.com/gr/latex?A%5En%3DM%20%5Cbegin%7Bbmatrix%7D%20(%5Cfrac%7B1%2B%5Csqrt%7B5%7D%7D%7B2%7D)%5En%260%5C%5C%200%26(%5Cfrac%7B1-%5Csqrt%7B5%7D%7D%7B2%7D)%5En%20%5Cend%7Bbmatrix%7D%20M%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20(%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D)%5E%7Bn-1%7D-(%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D)%5E%7Bn-1%7D%20%5Cright%5D%26%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20(%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D-(%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D%20%5Cright%5D%5C%5C%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20(%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D-(%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D%20%5Cright%5D%26%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20(%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D)%5E%7Bn%2B1%7D-(%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D)%5E%7Bn%2B1%7D%20%5Cright%5D%20%5Cend%7Bbmatrix%7D#card=math&code=A%5En%3DM%20%5Cbegin%7Bbmatrix%7D%20%28%5Cfrac%7B1%2B%5Csqrt%7B5%7D%7D%7B2%7D%29%5En%260%5C%5C%200%26%28%5Cfrac%7B1-%5Csqrt%7B5%7D%7D%7B2%7D%29%5En%20%5Cend%7Bbmatrix%7D%20M%5E%7B-1%7D%3D%20%5Cbegin%7Bbmatrix%7D%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20%28%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D%29%5E%7Bn-1%7D-%28%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D%29%5E%7Bn-1%7D%20%5Cright%5D%26%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20%28%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D-%28%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D%20%5Cright%5D%5C%5C%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20%28%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D-%28%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D%20%5Cright%5D%26%20%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20%28%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D%29%5E%7Bn%2B1%7D-%28%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D%29%5E%7Bn%2B1%7D%20%5Cright%5D%20%5Cend%7Bbmatrix%7D&id=J02av)
比较，可得 ![](https://g.yuque.com/gr/latex?F_n%3D%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20(%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D-(%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D)%5E%7Bn%7D%20%5Cright%5D#card=math&code=F_n%3D%5Cfrac%7B1%7D%7B%5Csqrt%7B5%7D%7D%5Cleft%5B%20%28%5Cfrac%7B1%2B%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D-%28%5Cfrac%7B1-%5Csqrt5%7D%7B2%7D%29%5E%7Bn%7D%20%5Cright%5D&id=iyNjv)


## 11 - 抽象向量空间

**行列式**和**特征向量**与所选坐标系无关；这二者都是暗含于空间中的性质

1. 函数实际上只是另一种向量

![](https://g.yuque.com/gr/latex?(f%2Bg)(x)%3Df(x)%2Bg(x)#card=math&code=%28f%2Bg%29%28x%29%3Df%28x%29%2Bg%28x%29&id=TNGXV) 和向量对应坐标相加相似（无数个坐标的相加）

![](https://g.yuque.com/gr/latex?(2f)(x)%3D2f(x)#card=math&code=%282f%29%28x%29%3D2f%28x%29&id=ZqZO0) 和向量对应坐标数乘相似

2. 函数的线性变换

函数的线性变换，这个变换接收一个函数，并把它变成另一个函数，例如求导；“**算子**” 和 “**变换**” 是一样的

**线性的严格定义**： ![](https://g.yuque.com/gr/latex?L(%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D)%3DL(%5Cvec%7Bv%7D)%2BL(%5Cvec%7Bw%7D)%2CL(c%5Cvec%7Bv%7D)%3DcL(%5Cvec%7Bv%7D)#card=math&code=L%28%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D%29%3DL%28%5Cvec%7Bv%7D%29%2BL%28%5Cvec%7Bw%7D%29%2CL%28c%5Cvec%7Bv%7D%29%3DcL%28%5Cvec%7Bv%7D%29&id=JYKbw) 【可加性和成比性（一阶齐次）】

一个函数变换是线性的？

eg. 求导是线性运算 ![](https://g.yuque.com/gr/latex?(f(x)%2Bg(x))'%3Df'(x)%2Bg'(x)%2C(af(x))'%3Daf'(x)#card=math&code=%28f%28x%29%2Bg%28x%29%29%27%3Df%27%28x%29%2Bg%27%28x%29%2C%28af%28x%29%29%27%3Daf%27%28x%29&id=jiJud)

用矩阵描述求导

当前空间为全体多项式；自然地，取 ![](https://g.yuque.com/gr/latex?1%2Cx%2Cx%5E2%2Cx%5E3%2C%5Cldots#card=math&code=1%2Cx%2Cx%5E2%2Cx%5E3%2C%5Cldots&id=W3Y5N) 为基（基函数）， ![](https://g.yuque.com/gr/latex?b_0(x)%3D1%2Cb_1(x)%3Dx%2C%5Cldots#card=math&code=b_0%28x%29%3D1%2Cb_1%28x%29%3Dx%2C%5Cldots&id=I5oLk) ，基函数集是无穷大的

eg. ![](https://g.yuque.com/gr/latex?1x%5E2%2B3x%2B5%5Ccdot1%3D%20%5Cbegin%7Bbmatrix%7D%205%5C%5C3%5C%5C1%5C%5C0%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D#card=math&code=1x%5E2%2B3x%2B5%5Ccdot1%3D%20%5Cbegin%7Bbmatrix%7D%205%5C%5C3%5C%5C1%5C%5C0%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D&id=OVKW0)

![](https://g.yuque.com/gr/latex?a_nx%5En%2Ba_%7Bn-1%7Dx%5E%7Bn-1%7D%2B%5Ccdots%2Ba_1x%2Ba_0%3D%20%5Cbegin%7Bbmatrix%7D%20a_0%5C%5Ca_1%5C%5C%5Cvdots%5C%5Ca_%7Bn-1%7D%5C%5Ca_n%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D#card=math&code=a_nx%5En%2Ba_%7Bn-1%7Dx%5E%7Bn-1%7D%2B%5Ccdots%2Ba_1x%2Ba_0%3D%20%5Cbegin%7Bbmatrix%7D%20a_0%5C%5Ca_1%5C%5C%5Cvdots%5C%5Ca_%7Bn-1%7D%5C%5Ca_n%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D&id=uTyS0)

![](https://g.yuque.com/gr/latex?%5Cfrac%7B%5Crm%20d%7D%7B%7B%5Crm%20d%7Dx%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%261%260%260%26%5Ccdots%5C%5C%200%260%262%260%26%5Ccdots%5C%5C%200%260%260%263%26%5Ccdots%5C%5C%200%260%260%260%26%5Ccdots%5C%5C%20%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cddots%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cfrac%7B%5Crm%20d%7D%7B%7B%5Crm%20d%7Dx%7D%3D%20%5Cbegin%7Bbmatrix%7D%200%261%260%260%26%5Ccdots%5C%5C%200%260%262%260%26%5Ccdots%5C%5C%200%260%260%263%26%5Ccdots%5C%5C%200%260%260%260%26%5Ccdots%5C%5C%20%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cddots%20%5Cend%7Bbmatrix%7D&id=G44bI)

eg. ![](https://g.yuque.com/gr/latex?%5Cfrac%7B%5Crm%20d%7D%7B%7B%5Crm%20d%7Dx%7D(1x%5E3%2B5x%5E2%2B4x%2B5)%3D%20%5Cbegin%7Bbmatrix%7D%200%261%260%260%26%5Ccdots%5C%5C%200%260%262%260%26%5Ccdots%5C%5C%200%260%260%263%26%5Ccdots%5C%5C%200%260%260%260%26%5Ccdots%5C%5C%20%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cddots%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%205%5C%5C4%5C%5C5%5C%5C1%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%5Ccdot4%5C%5C2%5Ccdot5%5C%5C3%5Ccdot1%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D#card=math&code=%5Cfrac%7B%5Crm%20d%7D%7B%7B%5Crm%20d%7Dx%7D%281x%5E3%2B5x%5E2%2B4x%2B5%29%3D%20%5Cbegin%7Bbmatrix%7D%200%261%260%260%26%5Ccdots%5C%5C%200%260%262%260%26%5Ccdots%5C%5C%200%260%260%263%26%5Ccdots%5C%5C%200%260%260%260%26%5Ccdots%5C%5C%20%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cvdots%26%5Cddots%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%205%5C%5C4%5C%5C5%5C%5C1%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D%3D%20%5Cbegin%7Bbmatrix%7D%201%5Ccdot4%5C%5C2%5Ccdot5%5C%5C3%5Ccdot1%5C%5C0%5C%5C%5Cvdots%20%5Cend%7Bbmatrix%7D&id=Qw8tI)

| 线性代数中的概念 | 应用于函数时的别名 |
| --- | --- |
| 线性变换 | 线性算子 |
| 点积 | 内积 |
| 特征向量 | 特征函数 |


3. 向量空间

**向量空间**：这些类似向量的事物，比如箭头、一组数、函数等，它们构成的集合被称为**向量空间**

如果要让所有建立好的理论和概念适用于一个向量空间，那么它必须满足八条公理

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%201)%5Cvec%7Bu%7D%2B(%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D)%3D(%5Cvec%7Bu%7D%2B%5Cvec%7Bv%7D)%2B%5Cvec%7Bw%7D%5C%5C%202)%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D%3D%5Cvec%7Bw%7D%2B%5Cvec%7Bv%7D%5C%5C%203)%5Cvec%7B0%7D%2B%5Cvec%7Bv%7D%3D%5Cvec%7Bv%7D%5C%5C%204)%5Cvec%7Bv%7D%2B(-%5Cvec%7Bv%7D)%3D%5Cvec%7B0%7D%5C%5C%205)a(b%5Cvec%7Bv%7D)%3Dab(%5Cvec%7Bv%7D)%5C%5C%206)1%5Cvec%7Bv%7D%3D%5Cvec%7Bv%7D%5C%5C%207)a(%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D)%3Da%5Cvec%7Bv%7D%2Ba%5Cvec%7Bw%7D%5C%5C%208)(a%2Bb)%5Cvec%7Bv%7D%3Da%5Cvec%7Bv%7D%2Bb%5Cvec%7Bv%7D%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D#card=math&code=%5Cbegin%7Bequation%7D%20%5Cbegin%7Barray%7D%7Bl%7D%201%29%5Cvec%7Bu%7D%2B%28%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D%29%3D%28%5Cvec%7Bu%7D%2B%5Cvec%7Bv%7D%29%2B%5Cvec%7Bw%7D%5C%5C%202%29%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D%3D%5Cvec%7Bw%7D%2B%5Cvec%7Bv%7D%5C%5C%203%29%5Cvec%7B0%7D%2B%5Cvec%7Bv%7D%3D%5Cvec%7Bv%7D%5C%5C%204%29%5Cvec%7Bv%7D%2B%28-%5Cvec%7Bv%7D%29%3D%5Cvec%7B0%7D%5C%5C%205%29a%28b%5Cvec%7Bv%7D%29%3Dab%28%5Cvec%7Bv%7D%29%5C%5C%206%291%5Cvec%7Bv%7D%3D%5Cvec%7Bv%7D%5C%5C%207%29a%28%5Cvec%7Bv%7D%2B%5Cvec%7Bw%7D%29%3Da%5Cvec%7Bv%7D%2Ba%5Cvec%7Bw%7D%5C%5C%208%29%28a%2Bb%29%5Cvec%7Bv%7D%3Da%5Cvec%7Bv%7D%2Bb%5Cvec%7Bv%7D%20%5Cend%7Barray%7D%20%5Cend%7Bequation%7D&id=lHMUB)

**向量的形式并不重要**，只要向量相加和数乘的概念遵守以上规则即可

> “普适的代价是抽象”Abstractness is the price of generality.


## 12 - 克莱姆法则，几何解释

1. 尝试

![](https://g.yuque.com/gr/latex?%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D%3Dx%5CnRightarrow%20T(%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D)%20T(%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D)%3Dx%5C%5C%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C1%20%5Cend%7Bbmatrix%7D%3Dy%5CnRightarrow%20T(%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D)%20T(%5Cbegin%7Bbmatrix%7D%200%5C%5C1%20%5Cend%7Bbmatrix%7D)%3Dy#card=math&code=%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D%3Dx%5CnRightarrow%20T%28%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%29%20T%28%5Cbegin%7Bbmatrix%7D%201%5C%5C0%20%5Cend%7Bbmatrix%7D%29%3Dx%5C%5C%20%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%20%5Cbegin%7Bbmatrix%7D%200%5C%5C1%20%5Cend%7Bbmatrix%7D%3Dy%5CnRightarrow%20T%28%5Cbegin%7Bbmatrix%7D%20x%5C%5Cy%20%5Cend%7Bbmatrix%7D%29%20T%28%5Cbegin%7Bbmatrix%7D%200%5C%5C1%20%5Cend%7Bbmatrix%7D%29%3Dy&id=Cfmdz)

**正交变换**： ![](https://g.yuque.com/gr/latex?%5Cforall%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D%2CT(%5Cvec%7Bv%7D)%5Ccdot%20T(%5Cvec%7Bw%7D)%3D%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D#card=math&code=%5Cforall%5Cvec%7Bv%7D%2C%5Cvec%7Bw%7D%2CT%28%5Cvec%7Bv%7D%29%5Ccdot%20T%28%5Cvec%7Bw%7D%29%3D%5Cvec%7Bv%7D%5Ccdot%5Cvec%7Bw%7D&id=wV9Yu) ，则 ![](https://g.yuque.com/gr/latex?T#card=math&code=T&id=qnPrP) 为**正交变换**（使基向量保持单位长度且相互垂直）

2. 几何转换 克莱姆法则

二维 ![](https://g.yuque.com/gr/latex?SignedArea%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%200%26x%5C%5C%201%26y%20%5Cend%7Bbmatrix%7D%7D%20%3D1%5Ctimes%20y#card=math&code=SignedArea%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%200%26x%5C%5C%201%26y%20%5Cend%7Bbmatrix%7D%7D%20%3D1%5Ctimes%20y&id=mz7ZU) （有向面积）

三维 ![](https://g.yuque.com/gr/latex?z%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%201%260%26x%5C%5C%200%261%26y%5C%5C%200%260%26z%20%5Cend%7Bbmatrix%7D%7D%2C%20y%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%201%26x%260%5C%5C%200%26y%260%5C%5C%200%26z%261%20%5Cend%7Bbmatrix%7D%7D%2C%20x%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20x%260%260%5C%5C%20y%261%260%5C%5C%20z%260%261%20%5Cend%7Bbmatrix%7D%7D#card=math&code=z%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%201%260%26x%5C%5C%200%261%26y%5C%5C%200%260%26z%20%5Cend%7Bbmatrix%7D%7D%2C%20y%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%201%26x%260%5C%5C%200%26y%260%5C%5C%200%26z%261%20%5Cend%7Bbmatrix%7D%7D%2C%20x%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20x%260%260%5C%5C%20y%261%260%5C%5C%20z%260%261%20%5Cend%7Bbmatrix%7D%7D&id=Q8U76)

应用变换后，所有面积伸缩的比例都等于给定的行列式

![](https://g.yuque.com/gr/latex?y%3D%5Cfrac%7BArea%7D%7B%7B%5Crm%20det%7D(A)%7D#card=math&code=y%3D%5Cfrac%7BArea%7D%7B%7B%5Crm%20det%7D%28A%29%7D&id=I6gvA)

三维及高维也是类似的

## 13 - 计算二阶矩阵特征值的妙计

1）矩阵的迹

![](https://g.yuque.com/gr/latex?tr%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5Cc%26d%20%5Cend%7Bbmatrix%7D%7D%3Da%2Bd%3D%5Clambda_1%2B%5Clambda_2#card=math&code=tr%3D%7B%5Crm%20det%7D%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5Cc%26d%20%5Cend%7Bbmatrix%7D%7D%3Da%2Bd%3D%5Clambda_1%2B%5Clambda_2&id=AMfjA)

![](https://g.yuque.com/gr/latex?%7B%5Crm%20mean%7D(a%2Cd)%3D%7B%5Crm%20mean%7D(%5Clambda_1%2B%5Clambda_2)#card=math&code=%7B%5Crm%20mean%7D%28a%2Cd%29%3D%7B%5Crm%20mean%7D%28%5Clambda_1%2B%5Clambda_2%29&id=U68EB)

2）（二阶）矩阵的行列式

![](https://g.yuque.com/gr/latex?det%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5Cc%26d%20%5Cend%7Bbmatrix%7D%7D%3Dad-bc%3D%5Clambda_1%5Clambda_2#card=math&code=det%5Cpmatrix%7B%20%5Cbegin%7Bbmatrix%7D%20a%26b%5C%5Cc%26d%20%5Cend%7Bbmatrix%7D%7D%3Dad-bc%3D%5Clambda_1%5Clambda_2&id=M8tWo)

3）

![](https://g.yuque.com/gr/latex?%5Cfrac%7B%5Clambda_1%2B%5Clambda_2%7D%7B2%7D%3Dm%2C%5Clambda_1%5Clambda_2%3Dp#card=math&code=%5Cfrac%7B%5Clambda_1%2B%5Clambda_2%7D%7B2%7D%3Dm%2C%5Clambda_1%5Clambda_2%3Dp&id=F26bf) 则 ![](https://g.yuque.com/gr/latex?%5Clambda_1%2C%5Clambda_2%3Dm%5Cpm%5Csqrt%7Bm%5E2-p%7D#card=math&code=%5Clambda_1%2C%5Clambda_2%3Dm%5Cpm%5Csqrt%7Bm%5E2-p%7D&id=goIhB)
