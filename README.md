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
### 绝对路径-从**盘符**出发查找目标文件

![image.png](attachment:68c48783-7bef-4eea-84d5-c69ab4d5c84b:image.png)

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
        <!-- 绝对路径访问图片 -->
        <img src="C:\Users\www12\Desktop\yjtp.png" alt="图片加载失败">
        <img src="C:/Users/www12/Desktop/yjtp.png" alt="图片加载失败">
    </body>
    </html>
    ```
    
    ![image.png](attachment:e357063e-5068-4acc-82cd-e0c855a48f0f:image.png)
    
- 直接填写在线网址的图片url地址
    - 代码演示
        
        ```html
            <img src="http://gips2.baidu.com/it/u=195724436,3554684702&fm=3028&app=3028&f=JPEG&fmt=auto?w=1280&h=960" alt="">
        
        ```
        
        ![image.png](attachment:e8e8fa35-f5c5-43a7-b2aa-5aee85778328:image.png)
        

### 友情链接

跟自己网站有关系的网站。

- 实现方式
    - 使用对应网站的在线网址，一般使用**绝对路径**

## 超链接

### 跳转网页链接

点击之后跳转页面

- 相关标签
    
    ```html
    <a href="https://www.baidu.com">跳转到百度</a>
    
    **<!--target="_blank"-->  该属性表示在新窗口跳转页面**
    ```
    
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <!-- 通过超链接跳转网站 -->
        <a href="https://www.baidu.com" target="_blank">跳转到百度</a>
    </body>
    </html>
    ```
    
    ![image.png](attachment:a6589ace-e555-4a61-9fad-ccdbc9d387e5:image.png)
    

### 跳转本地文件

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <!-- 通过超链接跳转网站 -->
      
        <a href="https://www.baidu.com" target="_blank">跳转到百度</a>
        **<a href="../250512/06-段落标签.html">跳转到06</a>**
    </body>
    </html>
    ```
    
    ![image.png](attachment:4b467384-0b42-4087-923c-00846dd36f00:image.png)
    

<aside>
💡

**在开发初期，不知道超链接的跳转地址，href属性值写#，表示空链接，不会跳转**

</aside>

- 代码演示

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- 通过超链接跳转网站 -->
    <a href="https://www.baidu.com" target="_blank">跳转到百度</a>
    <a href="../250512/06-段落标签.html">跳转到06</a>
    **<a href="#">空链接</a>**
</body>
</html>
```

![image.png](attachment:444e063c-74f3-4d9e-8b04-efd294ec869d:image.png)

## 音频标签

- 标签
    
    ```html
    <audio src="音频的URL"></audio>
    ```
    
- 常见属性
    
    
    | 属性 | 作用 | 特殊说明 |
    | --- | --- | --- |
    | **src（必须熟悉）** | **音频URL** | **支持格式：MP3、Ogg、Wav** |
    | controls | 显示音频控制面板 |  |
    | loop | 循环播放 |  |
    | autoplay | 自动播放 | 为了提升用户体验，浏览器一般会禁用自动播放功能 |
    
    ![image.png](attachment:4740f7e5-fcf6-464e-9376-2dbcdb9ab39f:image.png)
    
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
        <!-- 加载音频文件 -->
        **<!-- 在html5中，如果属性名与属性值完全一样，可以简写为一个单词-->**
        <audio src="./media/周杰伦-花海.mp3" controls></audio>
    </body>
    </html>
    ```
    
    ![image.png](attachment:05badbca-04c9-4c3b-880b-a9811cecd571:image.png)
    

## 视频标签

- 标签

```html
<video src="视频的URL"></video>
```

- 常见属性
    
    
    | 属性 | 作用 | 特殊说明 |
    | --- | --- | --- |
    | src（必须属性） | 视频URL | 支持格式MP4、WebM、Ogg |
    | controls | 显示视频控制面板 |  |
    | loop | 循环播放 |  |
    | muted | 静音播放 |  |
    | autoplay | 自动播放 | 为了提示用户体验，浏览器支持在**静音状态**自动播放 |
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=<device-width>, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <!-- 视频 -->
        <video src="./media/mda-na2gcpqhw9v8xn54.mp4" controls loop autoplay muted>视频</video>
    </body>
    </html>
    ```
    
    ![image.png](attachment:229d5229-eaf4-4c2f-8925-a9522f16b9d2:image.png)
    

## 案例1

<aside>
💡

网页制作的思路

**从上到下，先整体再局部，逐步分析制作**

分析内容→写代码→保存→刷新浏览器，看效果  写一个看一个

整体到局部的思路例如：先完成段落，再完成段落中的超链接

</aside>

- 案例代码
    
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <h1>案例1</h1>
        <hr>
        <p>在一片宁静的森林边缘，有一个小小的<a href="./17-案例2.html">村落</a>，村子里的房子错落有致地分布着，
            屋顶上的烟囱偶尔会冒出几缕轻烟，仿佛在诉说着家的温暖。
            村子中央有一口古老的井，传说这口井有着神奇的力量，
            能够实现诚心诚意之人的愿望。村民们虽然过着简单的生活，
            但他们彼此之间充满了关爱与帮助，每当夜幕降临，星空下的村子就会响起悠扬的歌声和孩子们欢快的笑声。
            在这个快节奏的世界里，这个小村落宛如一颗被遗忘的明珠，静静地散发着它独有的光芒，向每一个愿意聆听的人讲述着关于友情、爱与希望的故事。</p>
        <img src="./村庄.jpg" alt="图像无法加载" title="这是一个村庄" width="300">
        <h2>村庄介绍</h2>
        <p><ins>在这幅美丽的夜景图中，我们看到的是一个宁静而温馨的村庄。</ins><strong>村庄被茂密的森林环绕，仿佛与世隔绝，营造出一种神秘而又安详的氛围。夜幕降临，星空璀璨，点缀着深蓝色的天空，几朵轻盈的云彩悠然飘过。</strong>
    
    村庄中的房屋以传统的木结构为主，<em>屋顶覆盖着厚厚的茅草，烟囱中升起袅袅炊烟，透露出家的温暖和生活的气息。</em>每栋房子的窗户都透出柔和的灯光，照亮了周围的环境，让人感受到一种亲切和舒适。房屋之间的小径蜿蜒曲折，连接着每一户人家，显得格外和谐。
    
    在村庄的中心，有一个石砌的水井，周围摆放着几张简朴的长椅和桌子，村民们围坐在一起，享受着夜晚的凉爽和彼此的陪伴。孩子们在嬉戏玩耍，大人们则在交谈、喝茶或分享故事，整个场景充满了欢声笑语和家庭的温馨。
    
    这个村庄不仅是一个居住的地方，更是一个充满人情味和社区精神的家园。<del>在这里，时间似乎放慢了脚步，让人们能够远离城市的喧嚣，回归自然，享受简单而美好的生活。无论是那温暖的灯光，还是村民们之间的互动，都让人感受到一种深深的归属感和幸福感。</del></p>
        <h2>村庄人口</h2>
    </body>
    </html>
    ```
    
    ![image.png](attachment:fc43dcc2-166c-40a1-b14f-2c2c0b582c7f:image.png)
    

## 案例2-加入视频音频

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>美丽的<a href="./16-案例1.html" target="_blank">村庄</a></h1>
    <p>村庄被茂密的森林环绕，仿佛与世隔绝，营造出一种神秘而又安详的氛围。夜幕降临，星空璀璨，点缀着深蓝色的天空，几朵轻盈的云彩悠然飘过。</p>
    <h2>添加歌曲</h2>
    <audio src="./media/周杰伦-花海.mp3" controls ></audio>
    <h2>通过视频介绍村庄</h2>
    <p>村庄中的房屋以传统的木结构为主，屋顶覆盖着厚厚的茅草，烟囱中升起袅袅炊烟，透露出家的温暖和生活的气息。
        每栋房子的窗户都透出柔和的灯光，照亮了周围的环境，让人感受到一种亲切和舒适。房屋之间的小径蜿蜒曲折，连接着每一户人家，显得格外和谐。</p>
    <video src="./media/mda-na2gcpqhw9v8xn54.mp4" controls muted autoplay></video>
</body>
</html>
```

![image.png](attachment:6e9c015a-87fe-4953-a705-26620238bb2f:image.png)

# 第二天

## 列表、表格、表单

- 应用场景
    
    ![image.png](attachment:81fbaf89-4fdd-42d2-a1b9-7c7dbab221ab:image.png)
    

<aside>
💡

**三个标签都是嵌套关系**

</aside>

- 列表
    - 作用
        - 布局内容排列整齐的区域
    - 分类
        - 分为**无序列表（工作常用）**、有序列表、定义列表。
    
    ![image.png](attachment:69de7845-e8fa-46ba-8ff4-baedc790f635:image.png)
    
    - **无序列表**
        
        作用：布局排列整齐的不需要规定顺序的区域
        
        标签：
        
        ```html
        ul嵌套li，ul是无序列表，li是列表条目
        
        <ul>
        	<li>第一项</li>
        	<li>第二项</li>
        	<li>第三项</li>
        	......
        </ul>
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
                <ul>
                    <li>第一项</li> 独占一行
                    <li>第二项</li>
                    <li>第三项</li>
                </ul>
            </body>
            </html>
            ```
            
            ![image.png](attachment:f724198a-4ab0-4c6d-97e2-a89521d3a2e2:image.png)
            
        
        <aside>
        💡
        
        **ul标签里面只能包裹li标签**
        
        **li标签中可以包裹任意内容**
        
        </aside>
        
    - 有序列表
        
        作用：**布局排列整齐需要规定顺序的区域**
        
        ```html
        ol嵌套li，ol是有序列表，li是列表条目
        
        <ol>
        	<li>第一项</li>
        	<li>第二项</li>
        	<li>第三项</li>
        	......
        </ol>
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
                <ol>
                    <li>第一项</li>
                    <li>第二项</li>
                    <li>第三项</li>
                </ol>
            </body>
            </html>
            ```
            
            ![image.png](attachment:5b5dc767-4119-4671-a253-996eaa0f2851:image.png)
            
        
        <aside>
        💡
        
        **ul标签里面只能包裹li标签**
        
        **li标签中可以包裹任意内容**
        
        </aside>
        
    - 定义列表
        
        标签：dl嵌套dt和dd，dl是定义**列表**，dt定义**列表的标题**，dd是定义列表的**描述/详情**。
        
        ```html
        <dl>
        	<dt>列表标题</dt>
        	<dd>列表描述/详情</dd>
        	......
        </dl>
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
                <dl>
                    <dt>服务中心</dt>
                    <dd>申请售后</dd>
                </dl>
            </body>
            </html>
            ```
            
            ![image.png](attachment:2b1dc44c-a9db-40ea-95bf-f69e532aab07:image.png)
            
        
        <aside>
        💡
        
        **dl标签里面只能包裹dt和dd标签**
        
        **dt和dt标签中可以包裹任意内容**
        
        </aside>


