title: Markdown Syntax
date: 2015-10-10 10:03:21
tags:
---
Markdown学习练习笔记.
<!--more-->
方便读方便写,简单文本

可以使用html标签
块级标签用前后空行来隔开

	<table>
        <tr>
            <td>区块间的markdown格式语法不会处理</td><td>**但Haroopad预览会看到加粗了**</td>
        </tr>
	</table>

<table>
    <tr>
        <td>区块间的markdown格式语法不会处理</td><td>**但Haroopad预览会看到加粗了**</td>
    </tr>
</table>

	Head1|Head2|Head3
    ---|---|---
    姓名|性别|年龄
    张三|男|30
Head1|Head2|Head3
---|---|---
姓名|性别|年龄
张三|男|30

	&lt;&amp;> &copy;
    
&lt;&amp;> &copy;

### 标题
	H1
    ===
    H2
    ---
    # H1
    ## H2
    ### H3
    ###### H6

H1
===
H2
---------------------
### H3
###### H6

### 字体
	*斜体* **粗体** ***斜体加粗体***
	_斜体_  __粗体__ ___斜体加粗体___

*斜体* **粗体** ***斜体加粗体***
_斜体_  __粗体__ ___斜体加粗体___

### 区块引用
	>这个是区块引用
    >>A
    >>>* a
    >>>* b

>这个是区块引用
>>A
>>>* a
>>>* b

###代码

	public class User {
    	public static void main(String[] args) {
        	System.out.println("Hello World");
        }
    }

中间插入小块代码`code`,用反引号引起来`` ` ``.

需要插入反引号如 `` `哈哈` `` 使用``` `` `哈哈` `` ```

### 列表
无序列表`+`或`-`或`*`加空格
有序列表使用`数字`加`.`
	* A
	* B
	1. Hello
    world
    2. b
1. Hello
world
2. b

###转义
1986\. 这年

    \   反斜线
    `   反引号
    *   星号
    _   底线
    {}  花括号
    []  方括号
    ()  括弧
    #   井字号
    +   加号
    -   减号
    .   英文句点
    !   惊叹号


###分隔线

    ---
    ___
    ***
***



### 链接
	[链接文字](url "title")
另一种定义链接方式

	[链接文字][idName]
	[idName]:http://example.com "title可以放到下一行"
    或
    [链接文字][]
	[链接文字]:http://example.com "title可以放到下一行"

直接链接<http://example.com> `<http://example.com>`

### 图片
与链接很相似,唯一不一样的就是在最前面需要一个感叹号`!`,没法设置宽高

