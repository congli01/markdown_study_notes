# Markdow

## part1 标题
### 使用=和-标记以及和二级标题
### 使用#号标记
使用#号表示1-6级标题，一级标题一个#号，二级标题两个#号，以此类推


## part2 段落格式
### 段落
### 字体
*斜体*
_斜体_
**粗体**
__粗体__
***粗斜体***
___粗斜体___
### 分割线
第一行
***
第二行
* * *
第三行
- - -
第四行
*****
### 删除线
~~Microsoft~~
### 下划线
<u>Google</u>

### 脚注
创建脚注[^RUNOOB]
[^RUNOOB]:菜鸟教程


## part3 列表
### 无序列表
* 第一项
* 第二项
+ 第一项
+ 第二项
- 第一项
- 第二项
### 有序列表
1. 第一项
2. 第二项
10. 第三项（前面标号可以不按顺序）
### 列表嵌套
1. 第一项：
    - 嵌套1
    - 嵌套2
2. 第二项
    * 嵌套1
    * 嵌套2


## part3 区块
### 基本用法
> 区块引用
> Markdown区块
> 在段落开头使用>符号加空格
### 区块嵌套
> outer
> 外层区块
>> inner
>> 第一层嵌套
### 区块中使用列表
> block
> 1. first
> 2. second
> - 第一项
> - 第二项
### 列表中使用区块
- first
    > block
- second

## part4 代码
使用反引号(`)包起来，例如：

`printf()`函数

代码区块使用4个空格或这一个制表符

    public void print(String content) {
        System.out.println(content)
    }

```java
public void print(String content) {
    System.out.println(content)
}
```


## part5 链接
名称加地址：[菜鸟教程](https://www.runoob.com)

直接用地址：<https://github.com>

高级链接：
这个链接用1作为网址变量[Google][1]
这个链接用runoob作为网址变量[Runoob][runoob]
然后在文档解为为变量赋值
<!-- 注意空一行 -->
[1]: https://www.google.com
[runoob]: https://www.runoob.com


## part6 图片
语法格式：

    ![alt 属性文本](图片地址)
    ![alt 属性文本](图片地址 "可选标题")

![picture](https://th.bing.com/th/id/R.b030f39cf1be003992d1b72cd90dd921?rik=vCqPy0lPGNtYAA&riu=http%3a%2f%2fwww.kutoo8.com%2fupload%2fimage%2f17895398%2f201305161015.jpg&ehk=C8dqQ9iYAUSocnc2jKzS5ut5JXhrEbJ3sCB4w%2fckNYM%3d&risl=&pid=ImgRaw&r=0)

或者：

这个链接用2作为网址变量[picture][2]
然后在文档的结尾为变量赋值

[2]: https://desk-fd.zol-img.com.cn/t_s960x600c5/g5/M00/02/04/ChMkJ1bKyA2IUt_bAAvPNhi8QSoAALH8gHIUicAC89O906.jpg

    Markdown还没有办法指定图片的高度与宽度，如果需要，可以使用普通的<img>标签

<img src="https://desk-fd.zol-img.com.cn/t_s960x600c5/g5/M00/02/04/ChMkJ1bKyA2IUt_bAAvPNhi8QSoAALH8gHIUicAC89O906.jpg" width = 100%>


## part7 表格
使用|来分隔不同的单元格，使用-来分隔表头和其他行

|表头1|表头2|表头3|
|----|----|----|
|单元格|单元格|单元格|

对齐：
| 左对齐 | 右对齐 | 居中对齐 |
| :---- | ----: | :----: |
|左|右|中|


## part8 高级技巧
- 支持的HTML元素
- 转义
**文本加粗**
\*\*文本加粗\*\*
- 公式
```
$...$或者\(...\)中的数学表达式会在行内显示
$$...$$或者\[...\]或者```math中的数学表达式会在块内显示
```
$$
\begin{Bmatrix}
    a & b \\
    c & d
\end{Bmatrix}
$$