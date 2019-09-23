## Markdown 基础语法
Markdown是一种纯文本的轻量级标记语言，可用于表达富文本信息  
你现在看到的这份文档就是用markdown来书写的  
[查看代码](https://raw.githubusercontent.com/sgsq/train/master/md.md)  
我们提供[在线markdown编辑器](./tool/editor.html)  
你可以下载markdownpad2用于编写markdown文件。

### 标题
六个或以上 '=' 可以产生一个H1

    This is an H1
    ======
    
This is an H1
======

六个或以上下划线可以产生一个H2

    This is an H2
    ------
    
This is an H2
------

H1到H6分别可以用#号表示

# H1
## H2
### H3
#### H4
##### H5
###### H6

    # H1
    ## H2
    ### H3
    #### H4
    ##### H5
    ###### H6

### 段落与行
用一个空行或者是一个只包含空格和制表符，那种看起来像空行的行来分段。

    para.1
    
    para.2
    
para.1

para.2

在行末加两个或两个以上的空格，可以用来强制换行。

    line 1  
    line 2
    
line1  
line 2

### 引用
使用>来实现引用

    > lorem

> lorem

可以试着多层引用

    > lorem
    >> ipsum
    >>> dolor

> lorem
>> ipsum
>>> dolor

### 强调
使用两个星号或者两个下划线来加粗

    **bold**
    __bold__


**bold**
__bold__

使用一个新号和一个下划线来倾斜。

    *italic*
    _italic_

*italic*
_italic_

markdown本身不支持删除标签，请使用html

<pre>This is a <del>black</del> black and white cat.</pre>
    
This is a <del>black</del> black and white cat.

### 列表
使用*创建无序列表

    * Red
    * Green
    * Blue

* Red
* Green
* Blue

使用数字和点创建有序列表

    1. A
    2. B
    3. C

1. A
2. B
3. C

请注意列表与表示数字无关
上面的例子还可以这样写

    1. A
    1. B
    1. C

甚至是这样

    3. A
    2. B
    8. C
    
这几种方法的输出是相同的

### 水平线
以下代码都能产生水平线
<pre>

   ------
   
   ***
   
   * * *
   
   *****
</pre>

------

### 插入图片
请使用图床上传图片
    
    ![logo](https://i.loli.net/2019/09/24/fwhMnmrXDz9pHNG.jpg)

![logo](https://i.loli.net/2019/09/24/fwhMnmrXDz9pHNG.jpg)

### 链接
使用 \[text\]\(url title\) 创建链接

    Click [here](# "more") for more information.
     
Click [here](# "more") for more information.

### 代码行与代码块
用单引号来产生一个代码行

    Please use 'alert()' to debug.

Please use 'alert()' to debug.

用四个空格来产生代码块。

        #include<cstdio>
        using namespace std;
        int main()
        {
        printf("Hello world")
        }
        return 0;
        
    #include<cstdio>
    using namespace std;
    int main()
    {
    printf("Hello world"
    }
    return 0;
    
### 反斜杠转义
如果想要输出'* * *'而不是一条水平线应该怎样做
使用反斜杠使系统忽略原来符号的意思

    \* \* \*
    
\* \* \*

### 自动链接
如果要让一个链接可以被点击同时显示这个链接如果要让一个链接可以被点击同时显示这个链接文本应该怎样做
我们当然可以用这种方法。

    ![https://sgsq.github.io](https://sgsq.github.io)
    
但有比这更好的处理方法

    <https://sgsq.github.io>
    
<https://sgsq.github.io>
