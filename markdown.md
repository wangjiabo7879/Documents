# markdown基本语法知识

### 一、标题

- 一级标题：#
- 二级标题：##
- 三级标题：###
- 四级标题：####
- 五级标题：#####
- 六级标题：######

### 二、段落格式

 markdown段落没有特殊的格式，直接编写文本。

1. 字体

   ```python
   """
   1、斜体：*123*
   2、粗体：**123**
   3、粗斜体：***123***
   """
   ```

   

   + 斜体：*123*

   + 粗体：**123**

   + 粗斜体：***123***

     

2. 分隔线

   在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他的内容。

   例如：

   - 星号：***、---、+++、_ _ _

     ***

     ---

     ___

     +++

3. 删除线

   ```python
   # 在文字两端添加~~
   ```

   例子：~~添加删除线~~

4. 下划线

   ```python
   # 通过HTML的<u>来实现
   # <u>下划线</u>
   ```

   <u>下划线</u>

5. 脚注

   ```python
   # 脚注是对文本的补充说明
   # 格式：[^要注释的文本]
   ```

   《游山西村》[^注释①]

### 三、区块

```python
# 在段落开头使用 > 符号
```

> 区块line
>
> .....
>
> .....

```python
# 区块嵌套
```

> 最外层
>
> > 第二层
> >
> > > 第三层

```python
# 区块中的列表
```

>在区块中使用列表
>
>1. 第一项
>2. 第二项
>
>- 第三项
>- 第四项

```python
# 在列表中使用区块
```

1. 列表

   > line1
   >
   > line2
   >
   > > line3

2. 列表

### 四、列表

1. 无序列表标记

```java
/** 以下三种表达方式效果一致：
	* 第一项
	* 第二项
	* 第三项
	
	+ 第一项
	+ 第二项
	+ 第三项
	
	- 第一项
	- 第二项
	- 第三项
*/
```

* 第一项
* 第二项
* 第三项

2. 有序列表标记

   ```java
   // 有序列表使用数字加上.号来表示
   /*	1. 第一项
   	2. 第二项
   	3. 第三项
   */
   ```

   1. 第一项
   2. 第二项
   3. 第三项

3. 列表嵌套

   ```java
   // 列表嵌套只需要在子列表中的选项前面添加四个空格即可
   /**
   	1. 第一项
   	    - 元素1
   	    - 元素2
   	2. 第二项
   	    - 元素1
   	    - 元素2
   */
   ```

   1. 第一项
         - 元素1
         - 元素2
   2. 第二项
         - 元素1
         - 元素2

### 五、代码

```python
# 在函数函数或者片段的代码使用反引号抱起来
'''
	`printf()`
	`printf();a=b+c`
'''
```

`printf()`

`printf();a=b+c`

```java
// 代码区块
/* 格式：三个反引号加上编程语言
···python
```

```python
import requests
print("I am a python program!")
```

### 六、链接

```java
/*
格式1：[链接名称](链接地址)
格式2: <链接地址>
*/
```

- 格式1：[Google](www.google.com)

- 格式2：<www.google.com>

```java
// 高级链接：通过变量来设置一个链接，变量赋值在文档末尾进行
/*
	Google链接为[Google](var1)
	Google链接为[Google](var2)
*/
```

### 七、图片

```java
/* Form:
	![alt 属性文本](图片地址)
	![alt 属性文本](图片地址 “可选标题”)
*/
```

<img src="F:\01-Project\GitProject\Documents\images\windows.png" alt="123 窗户" style="zoom:33%;" />

<img src="F:\01-Project\GitProject\Documents\images\windows.png" alt="123 窗户" title="鼠标位置在这儿 " style="zoom:25%;" />

### 八、表格

直接插入，使用代码麻烦！

### 九、公式

```python
'''
格式：$$,回车即可进入公式编辑
'''
# 可以导入外部公式代码
"""		
$$
\mathbf{V}_1 \times \mathbf{V}_2 = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\\frac{\partial X}{\partial u} & \frac{\partial Y}{\partial u} & 0 \\\frac{\partial X}{\partial v} & \frac{\partial Y}{\partial v} & 0 \\\end{vmatrix}${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$

"""
```


$$
x^2+Y^2=c^3
$$

$$
\mathbf{V}_1 \times \mathbf{V}_2 = \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} & \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} & \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$

[^注释①]: 宋代陆游著作。

[var1]: http://www.google.com
[var2]: http://www.fake.com