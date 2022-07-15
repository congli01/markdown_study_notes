# Markdow

## 标题

---

1. =号与-号标识  
    在文本下方添加任意数量的=标识一级标题
2. #号标识  
    使用#号表示1-6级标题，一级标题一个#号，二级标题两个#号，以此类推


## 段落

---
 
1. 换行  
    - HTML的`<br>`标签
    - 两个或多个空格（vscode的Markdown Preview Enhanced插件貌似渲染不出来？）

2. 段落  
    使用空白行将一行或多行文本进行分隔
    不要用空格或制表符缩进段落

3. 字体  
    - 斜体
    在单词或短语前后各添加1个*或_  
    *斜体*        _斜体_
    - 粗体
    在单词或短语前后各添加2个*或_  
    **粗体**    __粗体__   
    Markdown应用程序如何处理单词或短语间的下划线上并不一致，为了兼容性，在单词或短语中间部分加粗时使用`*`  B**ol**d  
    - 粗斜体  
    3个*或_  
    ***粗斜体***    ___粗斜体___

4. 分割线   
    在单独一行使用三个或多个破折号（`---`）或星号（`***`）或下划线（`___`）作分割线  
    为了兼容性，在分割线前后均添加空白行

5. 删除线  
    在前后添加两个`~`  
    ~~删除线~~

6. 下划线  
    \<u>需要内容\</u>  
    <u>下划线</u>

7. 高亮  
    前后添加2个`=`  
    ==高亮==

8. 脚注  
    RUNOOB[^RUNOOB]  

    [^RUNOOB]:菜鸟教程  


## 列表

---

1. 无序列表  
    在每个列表项前面添加`-`、`*`或者`+`
    * 第一项
    * 第二项
    + 第一项
    + 第二项
    - 第一项
    - 第二项

2. 有序列表  
    在每列表项前添加数字并紧跟一个英文句点，数字不必按数学顺序排列，但需以1起始
    1. 第一项
    20. 第二项
    10. 第三项（前面标号可以不按顺序）


3. 列表嵌套  
    在子列表前添加四个空格  
    1. 第一项：
        - 嵌套1
        - 嵌套2
    2. 第二项
        * 嵌套1
        * 嵌套2


## 区块

---

1. 基本用法  
    > 区块引用
    > Markdown区块
    > 在段落开头使用>符号加空格

2. 区块嵌套  
    一个`>`是最外层，两个`>`是第一层嵌套，一次类推
    > outer
    > 外层区块
    >> inner
    >> 第一层嵌套

3. 区块中使用列表  
    ```
    > block
    > 1. first
    > 2. second
    > - 第一项
    > - 第二项
    ```

    > block
    > 1. first
    > 2. second
    > - 第一项
    > - 第二项

4. 列表中使用区块  
- first
    > block
- second


## 代码

---

1. 使用反引号(`)包起来，例如:  

    `printf()`函数

2. 代码区块使用4个空格或这一个制表符  

    public void print(String content) {
        System.out.println(content)
    }

3. 由` ``` `包裹一段代码，指定一种语言可实现代码高亮（也可以不指定，但无高亮）  
```java
public void print(String content) {
    System.out.println(content)
}
```


## part6 链接

---

1. `[显示名](地址)`：[菜鸟教程](https://www.runoob.com)

2. 直接用地址 `<地址>`：<https://github.com>

3. 高级链接：
    ```
    这个链接用1作为网址变量[Google][1]
    这个链接用runoob作为网址变量[Runoob][runoob]
    然后再为变量赋值
    <!-- 空一行 -->
    [1]: https://www.google.com
    [runoob]: https://www.runoob.com
    ```
    效果：  
    这个链接用1作为网址变量[Google][1]
    这个链接用runoob作为网址变量[Runoob][runoob]
    然后再为变量赋值
    <!-- 空一行 -->
    [1]: https://www.google.com
    [runoob]: https://www.runoob.com


## 图片

---

1. 语法格式：
    ```
    ![替代文本](图片链接)
    ![替代文本](图片链接 "可选标题")
    ```

![picture](https://th.bing.com/th/id/R.b030f39cf1be003992d1b72cd90dd921?rik=vCqPy0lPGNtYAA&riu=http%3a%2f%2fwww.kutoo8.com%2fupload%2fimage%2f17895398%2f201305161015.jpg&ehk=C8dqQ9iYAUSocnc2jKzS5ut5JXhrEbJ3sCB4w%2fckNYM%3d&risl=&pid=ImgRaw&r=0)

2. Markdown还没有办法指定图片的高度与宽度，如果需要，可以使用普通的`<img>`标签

<img src="https://desk-fd.zol-img.com.cn/t_s960x600c5/g5/M00/02/04/ChMkJ1bKyA2IUt_bAAvPNhi8QSoAALH8gHIUicAC89O906.jpg" width = 100%>


## 表格

---

使用|来分隔不同的单元格，使用-来分隔表头和其他行

|表头1|表头2|表头3|
|----|----|----|
|单元格|单元格|单元格|

对齐：
| 左对齐 | 右对齐 | 居中对齐 |
| :---- | ----: | :----: |
|左|右|中|


## 高级技巧

---

1. 支持的HTML元素

2. 转义
    **文本加粗**
    \*\*文本加粗\*\*

3. 任务列表 
    在任务列表项之前添加`-`和`[(空格)]`
    `- [x] 标题`
    `- [ ] 表格`
    `- [ ] 任务列表`
    - [x] 标题
    - [ ] 表格
    - [ ] 任务列表

4. 使用Emoji表情  
    - 复制粘贴表情符号  
    - 使用表情符号简码：以冒号开头和结尾并包含表情符号的名称  
    `:joy:`  :joy:  
    [表情符号简码列表](https://gist.github.com/rxaviers/7360908) （因应用程序而异）

5. 公式
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

    $$\lim_{x \to 0} sin(x) = 0 $$

---

参考：  
[菜鸟教程-markdown教程](https://www.runoob.com/markdown/md-tutorial.html)  
[markdown官方教程](https://markdown.com.cn/)
