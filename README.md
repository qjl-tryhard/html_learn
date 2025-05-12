# 第一天

## 开发环境

vscode   ctrl + + 放大字体

安装open in brower，设置谷歌为默认浏览器

Chrome

## HTML初体验

html为超文本标记语言，其中超文本就是链接，标记也叫标签，表示带尖括号的文本。

- 标签语法
    
    ![image.png](attachment:6dc75165-059f-4662-8759-567301bab803:image.png)
    
    - 标签成对出现，中间包裹内容
    - <>里面放英文字母（标签名）
    - 结束标签比开始标签多 /
    - 扩展
        - 双标签：成对出现的标签
        - 单标签：只有开始标签，没有结束标签
            - <br>: 换行
            - <hr>: 水平线
        - 如何区分单双标签？
            
            答：需要包裹内容的一般就是双标签，单标签例如下划线，换行等都是单标签。
            
    
    ![image.png](attachment:1d893db6-6ca6-419e-8bd7-e2116aa75f27:image.png)
    

## HTML基本骨架

```html
<html>
	<head>
		<title>网页标题</title>
	</head>
	<body>
		网页主体
	</body>
</html>
```

- html: 整个网页
- head: 网页头部，存放给浏览器看的代码，例如CSS
- body: 网页主题，存放给用户看的代码，例如 图片、文字

<aside>
💡

vscode快速生成：

在.html文件中，按英文状态下的感叹号！，加上Enter/Tab键进行生成。

</aside>

## 标签的关系

作用：明确代码的书写位置

- 父子关系（嵌套关系）
- 兄弟关系（并列关系）
    
    ![image.png](attachment:2a782a8a-cf46-4b03-9aa7-ce437739fc2c:image.png)
    
- 例子：
    - html标签对于head标签来说是父级关系
    - head与body是兄弟关系

## 注释

- 作用
    
    注释就是对代码的解释和说明，其目的是让人们能够更加轻松地了解代码。注释是编写程序时，写程序的人给一个语句、程序段、函数等的解释或提示，能提高程序代码的可读性。
    
    在编写HTML代码时，我们经常要在一些关键代码旁做一下注释，这样做的好处很多，比如：方便理解、方便查找或方便项目组里的其他程序员了解你的代码，而且可以方便以后你对自己代码进行修改。
    
    <aside>
    💡
    
    **学习和工作中，关键代码都要加注释！添加的注释并不会在浏览器中显示**
    
    </aside>
    
- 注释写法
    
    ```html
    <!-- 注释内容 -->
    
    快捷键
    ctrl + /
    ```
    

## 标题标签

一般用在新闻标题、文章标题、网页区域名称、产品名称等等

- 标签名
    
    ```html
    <h1> </h1> ~ <h6> </h6> (双标签)
    
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <h1>一级标题</h1> **独占一行，并且换行**
        <h2>二级标题</h2> **独占一行**
        <h3>三级标题</h3> **独占一行**
        <h4>四级标题</h4> **独占一行**
        <h5>五级标题</h5> **独占一行**
        <h6>六级标题</h6> **独占一行**
    </body>
    </html>
    ```
    
    ![image.png](attachment:c9c4766a-c443-4d6c-af25-5c64c56ecba0:image.png)
    
    <aside>
    💡
    
    **h1 标签在一个网页中只能用一次，用来放新闻标题（主标题）或网页的logo。h2-h6没有使用限制。**
    
    </aside>
    
    ![image.png](attachment:a828367a-bbaa-488f-b9f4-13a91c9cbc70:image.png)
    

## 段落标签

一般用在新闻段落、文章段落、产品描述信息等等。

- 段落标签写法
    
    ```html
    <p>(双标签)
    ```
    
    - 显示特点：
        - 独占一行
        - 两行之间有间隙
- 演示效果
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <p>2025年5月7日至10日，国家主席习近平应邀对俄罗斯进行国事访问并出席纪念苏联伟大卫国战争胜利80周年庆典。</p>
        <p>在百年变局加速演进、国际局势变乱交织背景下，此访回望历史、着眼未来，传承友谊、捍卫正义，取得圆满成功。一条大国、邻国关系发展的新路，穿越时光之门，从历史深处走向壮阔未来。</p>
    </body>
    </html>
    ```
    
    ![image.png](attachment:cb5c14a3-41ac-4b77-b53b-47ca28744ea3:image.png)
    

## 换行与水平线标签

html中无法使用Enter实现换行

- 代码执行效果
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        第一行内容
        <br>
        第二行内容
    
        测试
        <hr>
        1234567890
    </body>
    </html>
    ```
    
    ![image.png](attachment:5f4a3bb1-b026-4b64-b142-1ed0e485bb58:image.png)
    

## 文本格式化标签

- 作用：
    - 为文本添加特殊格式，用来**突出重点**。常见的文本格式：**加粗**、*倾斜*、下划线、~~删除线~~
- 标签主要部分有：
    1. 开始标签 <p>
    2. 结束标签 </p>
    3. 内容
- 具体
    
    
    | 标签名 | 效果 |
    | --- | --- |
    | strong | **加粗** |
    | em | *倾斜* |
    | ins | 下划线 |
    | del | ~~删除线~~ |
    
    | 标签名 | 效果 |
    | --- | --- |
    | b | **加粗** |
    | i | *倾斜* |
    | u | 下划线 |
    | s | ~~删除线~~ |
    
    <aside>
    💡
    
    工作中一般都是以左侧表格中的内容：
    
    因为这些标签自带**强调含义（语义）。**
    
    </aside>
    
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <strong>strong 加粗</strong>
        <br>
        <b>b 加粗</b>
        <br>
        <em>em 倾斜</em>
        <br>
        <i>i倾斜</i>
        <br>
        <ins>ins 下划线</ins>
        <br>
        <u>u 下划线</u>
        <br>
        <del>del 删除</del>
        <br>
        <s>s 删除</s>
    </body>
    </html>
    ```
    
    ![image.png](attachment:b97048fa-017e-4345-9b9f-1ba27c2cd77f:image.png)
    

## 图像标签-基本使用

- 作用：
    - 在网页中插入图片
- 使用
    
    ```html
    <img src="图片的URL">
    **# src用于指定图像的位置与名称，是图像标签必须的参数**
    ```
    
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
            <!-- alt的属性: 图片显示失败时出现的文字 
            并且多张图像不换行 
            ./可激活vscode的提示功能
        -->
        <img src="./yjtp.pngs" alt="图片加载失败">
    </body>
    </html>
    ```
    
    ![image.png](attachment:5459c8d9-2ae3-4397-87bb-30cbfc88f37d:image.png)
    

## 图像标签-属性

![image.png](attachment:04d676c6-591c-45a7-8351-6fea95f15b9a:image.png)

- 属性名 = “属性值”
- 属性写在**尖括号里面，属性名后面**，标签名和属性之间用**空格**隔开，不区分先后顺序

| 属性 | 作用 | 说明 |
| --- | --- | --- |
| alt | 替换文本 | 图片无法显示的时候显示的文字 |
| title | 提示文本 | 鼠标悬停在图片上面的时候显示的文字 |
| width | 图片的宽度 | 值为数字，没有单位 |
| height | 图片的高度 | 值为数字，没有单位 |

<aside>
💡

一般设置宽度和高度都是以CSS，重点关注前两个。并且浏览器默认是等比例缩放

</aside>

- 代码演示
    
    ```html
    <!-- 其他属性 -->
     <!DOCTYPE html>
     <html lang="en">
     <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
     </head>
     <body>
        <img src="./yjtp.png" alt="图片加载失败" title="这是一张图片" width="600">
     </body>
     </html>
    ```
    
    ![image.png](attachment:784cd753-2c59-431f-9ae9-8dc62ff3581c:image.png)
    
    定义宽度演示图片
    
    ![image.png](attachment:63847c10-ddd5-4c8c-b9fe-8585c8abc41c:image.png)
    

## 路径

路径指的是查找文件时，从起点到终点经历的路线。

- 路径分类
    - 相对路径：从**当前文件位置**出发找目标文件
    - 绝对路径：从**盘符**出发查找目标文件
        - Windows电脑从盘符出发
        - Mac电脑从根目录出发

<aside>
💡

**工作中大部分都是使用相对路径查找文件！**

</aside>

- 案例
    
    ![image.png](attachment:acef8257-e173-491b-8f93-c7c568336bd0:image.png)
    
    - ../表示进入了上一级目录   ../../进入上上一级目录
- 演示
    
    ![image.png](attachment:6f6441ab-fdcd-4bfa-88e5-b709e9d44a9a:image.png)
    

### 绝对路径-从**盘符**出发查找目标文件
