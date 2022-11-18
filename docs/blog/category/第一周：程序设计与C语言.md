# 程序设计与C语言

## 计算机和编程语言

计算机是怎么做事情的，编程语言是什么？

计算机如何解决问题

![](https://img-blog.csdnimg.cn/4972024e29ea4cc6844676b409d692ef.png#crop=0&crop=0&crop=1&crop=1&id=CdIiC&originHeight=542&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

## 计算机语言

程序是用特殊的编程语言写出来表达如何解决问题的

不是用编程语言来和计算机交谈，而是描述要求它如何做事情的过程或方法

## 计算机的语言

![](https://img-blog.csdnimg.cn/8b7357f5c41448eca4b0d20750a4a65a.png#crop=0&crop=0&crop=1&crop=1&id=iHRci&originHeight=615&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

计算机-程序-算法
![](https://img-blog.csdnimg.cn/2300d69a07e44bd0a96d944ae1d38588.png#crop=0&crop=0&crop=1&crop=1&id=dWO8M&originHeight=710&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)



## 算法

我们要让计算机做计算，就需要像这样找出计算的步骤，然后用编程语言写出来

计算机做的所有的事情都叫做计算

计算的步骤就是算法

## 计算机的思维方式

重复是计算机最擅长的

## 程序的执行

解释：借助一个程序，那个程序能试图理解你的程序，然后按照你的要求执行

编译：借助一个程序，就像一个翻译，把你的程序翻译成计算机真正能懂的语言——机器语言——写的程序，然后，这个机器语言写的程序就能直接执行了

## 解释语言 vs 翻译语言

语言本身无编译/解释之分，常用的执行方式而已

解释型语言有特殊的计算能力

编译型语言有确定的运算性能

## C语言

#### 为什么是C

C语言在工业界占有重要地位，在很多领域无可替代

为什么是C？

![](https://img-blog.csdnimg.cn/51e1d25c481f451a95ae20841a2651d0.png#crop=0&crop=0&crop=1&crop=1&id=GLPEt&originHeight=771&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)



其他语言？

![](https://img-blog.csdnimg.cn/1b3d938874744039a6723e44ae4e7861.png#crop=0&crop=0&crop=1&crop=1&id=VSR15&originHeight=666&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

## C 语言简史

### C 语言起源

![](https://img-blog.csdnimg.cn/c827bcb6366840da9a835243778dd91f.png#crop=0&crop=0&crop=1&crop=1&id=jphQk&originHeight=946&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

C语言是从B语言发展而来的，B语言是从BCPL发展而来的，BCPL是从FORTRAN发展而来的

BCPL和B都支持指针间接方式，所以C也支持了

C语言还受到了PL/I的影响，还和PDP-II的机器语言有很大的关系

1973年3月，第三版的Unix上出现了C语言的[编译器](https://so.csdn.net/so/search?q=%E7%BC%96%E8%AF%91%E5%99%A8&spm=1001.2101.3001.7020)

1973年11月，第四版的Unix（System Four）发布了，这个版本是完全用C语言重新写的

### C的发展与版本-K&R

![](https://img-blog.csdnimg.cn/54aef269bdaf4b33afedba9f7931d2fb.png#crop=0&crop=0&crop=1&crop=1&id=Sevno&originHeight=663&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

### C的发展与版本-标准

1989年ANSI发布了一个标准——ANSI C

1990年ISO接受了ANSI的标准——C89

C的标准在1995年和1999年两次更新——C89和C99

所有的当代编译器都支持C99了

## 编程软件

C语言的编程软件选择太多，课程推荐Dev C ++

## C 语言的应用

C 语言是一种工业语言

![](https://img-blog.csdnimg.cn/0854e388db224bff8fa829069311ef33.png#crop=0&crop=0&crop=1&crop=1&id=Lt3LT&originHeight=446&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

## 推荐的编程软件

编译—>运行

C需要被编译才能运行，所以你需要编辑器和编译器或者IDE（集成开发环境）

### Dev C++（4.9 for Win7，5.0 for Win8）

免费、安装简单、不用建工程

### 其他选择

- MS Visual Studio Express（Windows）
- Xcode（Max OS X）
- Eclipse-CDT
- Geany（和MinGW一起）
- Sublime（和MinGW一起）
- vim/emacs（和MinGW一起）

## 第一个程序

### 第一个C程序

如何在Dev C++中编辑、编译和运行程序

```c


#include <stdio.h>

int main()
{
    printf("Hello World!\n");

    return 0;
}
```

### 详解第一个程序

程序框架、`printf`、出错怎么办

#### 程序框架

![](https://img-blog.csdnimg.cn/1f4feb89945c403a95c57ea93fd44601.png#crop=0&crop=0&crop=1&crop=1&id=pNOYB&originHeight=690&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

#### 输出

`printf("Hello Wordld!\n");`

`""`里面的内容叫做“字符串”，`printf`会把其中的内容原封不动地输出

`\n`表示要在输出的结果后面换一行

#### 程序中的错误

![](https://img-blog.csdnimg.cn/36f963f76f7c4e8291eb72c433b19583.png#crop=0&crop=0&crop=1&crop=1&id=rcAPY&originHeight=723&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

#### C语言的编译器不管空格，回车和缩进

![](https://img-blog.csdnimg.cn/cdee7cdaa0af47a392dada1fa5fdf7f5.png#crop=0&crop=0&crop=1&crop=1&id=zQOos&originHeight=1046&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

## 不要用中文！

中国学生还有一个极其常见的低级错误，就是用了中文输入法来输入程序。那些标点符号，在中文和英文可能看上去相似，但是对于计算机是完全不同的符号，如果你还开了全角标点的话，问题就更严重了

## 做计算

如何让程序输出算术结果

### 例子：

`printf("%d\n", 23+43);`，`printf("23+43=%d\n", 23+43);`

`%d`说明后面有一个整数要输出在这个位置上
`%d`整数
`%f`浮点数 float
`%lf`浮点数 doublet

### 四则运算

![](https://img-blog.csdnimg.cn/57d4b51a4422409f8bb5b12d2d122371.png#crop=0&crop=0&crop=1&crop=1&id=uFe3T&originHeight=738&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

## 命令行编译和执行

Mac OS X如何在命令行编辑、编译和运行C程序

![](https://img-blog.csdnimg.cn/b8c76db3cb7d41a092ef3f7a3e4c33b8.png#crop=0&crop=0&crop=1&crop=1&id=dYlzE&originHeight=629&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

![](https://img-blog.csdnimg.cn/67776075b2e34242881d1c0c37194625.png#crop=0&crop=0&crop=1&crop=1&id=Wtugp&originHeight=1048&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

编译快捷键：cmd + B

运行快捷键：shift + cmd + B

![](https://img-blog.csdnimg.cn/ea6d903a59464150a2a8c44c4a225346.png#crop=0&crop=0&crop=1&crop=1&id=rIdNd&originHeight=730&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)

`vi`有三种工作方式，刚进入是命令模式，输入`i`进入插入模式编辑代码，结束后输入`Esc`回到命令模式，输入`:wq`保存并退出

![](https://img-blog.csdnimg.cn/d6ba4d05125e4a1ba820c1bcf9785b8e.png#crop=0&crop=0&crop=1&crop=1&id=Epo9m&originHeight=253&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&status=done&style=none&title=)
