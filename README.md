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
## 表格

网页中的表格与Excel表格类似，用来**展示数据**

- 标签内容
    
    **table**嵌套**tr**，**tr**嵌套**td/th**
    
    | 标签名 | 说明 |
    | --- | --- |
    | table | 表格 |
    | tr | 行 |
    | th | 表头单元格 |
    | td | 内容单元格 |

<aside>
💡

提示：在网页中，**表格默认没有边框线**，使用**border**属性可以为表格添加边框线。

**快捷键复制：shift + alt +上下        在上方或下方复制**

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
        <table border="1px">
            <!-- 行 -->
            <tr>
                <th>姓名</th>
                <th>性别</th>
            </tr>
            <tr>
                <td>张三</td>
                <td>男</td>
            </tr>
        </table>
    </body>
    </html>
    ```
    
    ![image.png](attachment:faf428aa-5345-4177-81f2-68302558619d:image.png)
    

## 表格结构标签 - 了解

作用：用表格结构标签把内容划分区域，让表格结构更清晰，语义更清晰。（不显示在浏览器中，只为让结构更清晰。）

- 标签
    
    
    | 标签名 | 含义 | 特殊说明 |
    | --- | --- | --- |
    | thead | 表格头部 | 表格头部内容 |
    | tbody | 表格主题 | 主要内容区域 |
    | tfoot | 表格底部 | 汇总信息区域 |
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
        <table border="1px">
            <thead>
                <tr>
                    <th>姓名</th>
                    <th>语文</th>
                    <th>数学</th>
                    <th>总分</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>张三</td>
                    <td>99</td>
                    <td>100</td>
                    <td>199</td>
                </tr>
                <tr>
                    <td>李四</td>
                    <td>98</td>
                    <td>100</td>
                    <td>198</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td>总结</td>
                    <td>全市第一</td>
                    <td>全市第一</td>
                    <td>全市第一</td>
                </tr>
            </tfoot>
        </table>
    </body>
    </html>
    ```
    
    ![image.png](attachment:86cdc73d-8a2e-46e7-91f5-c28d409e5853:image.png)
    

## 合并单元格

作用：将**多**个单元格合并为一个单元格，以**合并同类信息**。

- 分类
    - 跨行合并
    - 跨列合并
- 操作步骤
    1. 明确要合并的目标
    2. 保留**最左或者最上**的单元格，添加属性（取值为**数字**，表示需要合并的**单元格数量**）
        
        跨行合并，保留**最上**单元格，添加属性**rowspan**
        
        跨列合并，保留**最左**单元格，添加属性**colspan**
        
    3. 删除其他单元格

<aside>
💡

**不能跨结构标签进行合并！！！**

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
        <table border="1px">
            <thead>
                <tr>
                    <th>姓名</th>
                    <th>语文</th>
                    <th>数学</th>
                    <th>总分</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>张三</td>
                    <td>99</td>
                    **<td rowspan="2">100</td>**
                    <td>199</td>
                </tr>
                <tr>
                    <td>李四</td>
                    <td>98</td>
                    **<!-- <td>100</td> -->**
                    <td>198</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td>总结</td>
                    **<td colspan="3">全市第一</td>
                    <!-- <td>全市第一</td> -->
                    <!-- <td>全市第一</td> -->**
                </tr>
            </tfoot>
        </table>
    </body>
    </html>
    ```
    
    ![image.png](attachment:1b46aac9-dfa3-4347-9f7b-76e958527bf1:image.png)
    

## 表单

- 作用：收集用户信息
- 使用场景：
    - 登录页面
    - 注册页面
    - 搜索区域

### input标签基本使用

- input标签**type属性值不同，则功能不同**。
    
    ```html
    <input type="...">
    ```
    
- type属性值及其说明
    
    
    | type属性值 | 说明 |
    | --- | --- |
    | text | 文本框，用于输入**单行**文本 |
    | password | 密码框 |
    | radio | 单选框 |
    | checkbox | 多选框 |
    | file | 上传文件 |
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>input的基本使用</title>
    </head>
    <body>
        输入框:<input type="text">
        <br><br>
        密码: <input type="password">
        <br><br>
        单选框: <input type="radio">
        <br><br>
        多选框：<input type="checkbox">
        <br><br>
        上传文件：<input type="file">
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:43882de2-5471-4fb8-a70d-2f748f50d1fa:image.png)
    

### input文本占位文本

类似下图：

![image.png](attachment:fb921a6d-b6bf-4a44-8042-e1322df712e6:image.png)

```html
<input type="..." placeholder="提示信息">
```

文本框与密码框都可以使用

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>input占位文本</title>
    </head>
    <body>
        文本框：<input type="text" placeholder="请输入用户名">
        <br><br>
        密码：<input type="password" placeholder="请输入密码">
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:93309fa3-5327-447b-88db-20f2b179f19d:image.png)
    

### 单选框 radio

- 常用属性
    
    
    | 属性名 | 作用 | 特殊说明 |
    | --- | --- | --- |
    | name | 控件名称 | 控件分组，同组只能选中一个（单选功能） |
    | checked | 默认选择 | 属性名和属性值相同，简写为一个单词 |
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>单选框 radio</title>
    </head>
    <body>
        <input type="radio" name="gender" checked> 男
        <input type="radio" name="gender"> 女
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:f38e2c2a-b36b-402f-bc36-e7f1ae3e70ee:image.png)
    

### 上传文件-file

默认情况下，文件上传表单控件只能上传一个文件，添加**multiple**属性可以实现**文件多选**功能

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>上传多个文件</title>
    </head>
    <body>
        上传文件：**<input type="file" multiple>**
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:6fb0ff95-edba-475e-b4b3-6fb7dead4885:image.png)
    

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>上传多个文件</title>
</head>
<body>
    上传文件：<input type="file" multiple>
    
</body>
</html>
```

### 多选框-checkbox

多选框也叫**复选框**

默认选中：**checked**

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
        <!-- 多选框默认选中功能 -->
        兴趣爱好：<input type="checkbox"> 敲代码
        <input type="checkbox" checked> 敲前端代码
        <input type="checkbox" checked> 敲前端Html代码
                
                
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:af88d902-5a99-4029-b545-f8a293956dde:image.png)
    

### 下拉菜单

节省页面空间

- 标签
    
    **select**嵌套option,**select是下拉菜单整体，option是下拉菜单的每一项**
    

![image.png](attachment:974eb379-5c0f-417d-839f-51c2a1170841:image.png)

<aside>
💡

**如果需要默认，则在某个option后加selected即可！！！**

</aside>

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>下拉框</title>
    </head>
    <body>
        <select>
            <option>北京</option>
            <option>上海</option>
            <option>徐州</option>
            <option>广州</option>
            <option selected>聊城</option>
        </select>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:90eba80c-8ec4-4405-bbd7-56892986cfb8:image.png)
    

### 文本域

作用：**多行**输入文本的表单控件

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>文本域</title>
    </head>
    <body>
        <!-- 右下角的拖拽功能在实际工作中会被禁用 
        并会使用CSS设计尺寸，而不是使用属性设置-->
        <textarea >请输入评论</textarea>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:eb5e36ef-6176-4daa-841c-535eb58db363:image.png)
    

### label标签

作用：网页中，某个标签的说明文本

![image.png](attachment:1f6fd8cd-1fea-4131-bf2c-b7d6d4aa60f8:image.png)

经验：用label标签绑定文字和表单控件的关系，**增大表单控件的点击范围**。

- 代码演示
    
    ```html
    第一种写法
    - label标签只包裹内容，不包裹表单控件
    - 设置label标签的**for**属性值和表单控件的**id**属性值**相同（增大点击范围）
    <input type="radio" id="man"> 
    <label for="man">男</label>**
    
    第二种写法
    - 使用label标签包裹文字和表单控件，不需要属性
    **<label><input type="radio">女</label>
    
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>label标签-增大点击范围</title>
    </head>
    <body>
        <input type="radio" name="gender" id="man">
        <label for="man">男</label>
        <!-- <input type="radio" name="gender" checked> 女 -->
        <label ><input type="radio" name="gender" checked>女</label>
    </body>
    </html>**
    
    ```
    

<aside>
💡

支持label标签增大点击范围的表单控件：**文本框、密码框、上传文件、单选框、多选框、下拉菜单、文本域**等等

</aside>

![image.png](attachment:27787673-8d83-4342-99fe-62f272cc8846:image.png)

### 按钮-button

作用：登录功能

- 标签
    
    ```html
    <button type="">按钮</button>
    ```
    
- type属性
    
    
    | type属性值 | 说明 |
    | --- | --- |
    | submit | 提交按钮，点击后可以提交数据到后台（默认功能） |
    | reset | 重置按钮，点击后将表单控件恢复默认值 |
    | button | 普通按钮，默认没有功能，一般配合Javascript使用 |
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
        **<!-- 都需要使用form表单包裹 
         action属性表示要提交到的地址-->
        <form action="">
        <!-- 创建输入框 -->
        用户名：<input type="text">
        <br>
        密码：<input type="password">
        <br>
        <!-- 创建按钮 -->
        <button type="submit">提交</button>
        <button type="reset">重置</button>
        <button type="button">按钮</button>
        </form>**
    </body>
    </html>
    ```
    
    ![image.png](attachment:6563f577-b9b2-441e-b4e1-ab7fb21639a2:image.png)
    

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- 都需要使用form表单包裹 
     action属性表示要提交到的地址-->
    <form action="">
    <!-- 创建输入框 -->
    用户名：<input type="text">
    <br>
    密码：<input type="password">
    <br>
    <!-- 创建按钮 -->
    <button type="submit">提交</button>
    <button type="reset">重置</button>
    <button type="button">按钮</button>
    </form>
</body>
</html>
```

## 无语义的布局标签

- 作用：**布局网页**（划分网页区域，摆放内容）
    - **div**：独占一行
    - **span**：不换行
- 标签
    
    ```html
    <div>div标签，独占一行</div>
    <span>span标签，不换行</span>
    ```
    
- 代码演示
    
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>无语义的标签布局-div/span</title>
    </head>
    <body>
        <!-- 独占一行的大盒子 -->
        <div>div标签</div>
        <div>div标签</div>
        <div>div标签</div>
        <!-- 不换行的小盒子 -->
        <span>span标签</span>
        <span>span标签</span>
        <span>span标签</span>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:ebf91598-1462-4dd7-9062-187baf6e63e0:image.png)
    

## 字符实体

作用：在网页中**显示预留字符**

例如：当敲多个空格时，浏览器只显示一个空格

要显示原<p>时

| 显示结果 | 描述 | 实体名称 |
| --- | --- | --- |
|  | 空格 | **&**nbsp; |
| < | 小于号 | &lt; |
| > | 大于号 | &gt; |
- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>字符实体</title>
    </head>
    <body>
        乾坤未定，你我皆是牛&nbsp;&nbsp;&nbsp;&nbsp;马
        <br>
        &lt;p&gt;
    </body>
    </html>
    ```
    
    ![image.png](attachment:c5f4fe79-7e92-47e9-b5cc-0540e7c96327:image.png)
    

## 综合案例-1

![image.png](attachment:29883441-165f-44eb-a47b-2ffb2545aacc:image.png)

![image.png](attachment:b744f6e8-d70b-4455-a70d-6236bb5148a8:image.png)
## 综合案例-2

注册信息的构建

- 代码实现
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>综合案例2</title>
    </head>
    <body>
        <!-- 注册信息的相关构建 -->
        <h1>注册信息</h1>
        <h2>个人信息</h2>
        <form>
            姓名：<input type="text" placeholder="请输入姓名">
            <br>
            <br>
            密码：<input type="password" placeholder="请输入密码">
            <br>
            <br>
            确认密码：<input type="password" placeholder="请再次输入密码">
            <br>
            <br>
            性别：<label><input type="radio" name="gender" > 男</label>
            <label><input type="radio" name="gender" checked> 女</label>
                <!-- <input type="radio" name="gender" checked> 女 -->
            <br>
            <br>
            居住城市：<select name="" id="">
                <option value="" selected>北京</option>
                <option value="">徐州</option>
                <option value="">南京</option>
                <option value="">聊城</option>
            </select>
    
            <h2>教育经历</h2>
            最高学历：<select name="" id="">
                <option value="" selected>博士</option>
                <option value="">硕士</option>
                <option value="">本科</option>
                <option value="">专科</option>
            </select>
            <br>
            <br>
            学校名称：<input type="text">
            <br>
            <br>
            所学专业：<input type="text">
            <br>
            <br>
            在校时间：<select name="" id="">
                <option value="">2015</option>
                <option value="">2016</option>
                <option value="">2017</option>
                <option value="">2018</option>
            </select>
            --
            <select name="" id="">
                <option value="">2019</option>
                <option value="">2020</option>
                <option value="">2021</option>
                <option value="">2022</option>
            </select>
    
            <h2>工作经历</h2>
            公司名称：<input type="text">
            <br>
            <br>
            工作描述：
            <br>
            <textarea name="" id="" ></textarea>
            <br>
            <br>
            <input type="checkbox">已阅读并同意以下协议：
            <ul>
                <li><a href="https://www.baidu.com">《用户服务协议》</a></li>
                <li><a href="https://www.baidu.com">《隐私政策》</a></li>
            </ul>
            <br>
            <br>
            <button type="submit">免费注册</button>
            <button type="reset">重新填写</button>
        </form>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:96b38ab2-70a4-479f-ada7-0ed1eb646903:image.png)
    

# 第三天 CSS的学习

## CSS初体验

- 定义
    
    **层叠样式表**，是一种**样式表**语言，用来描述**HTML文档的呈现（美化内容）**。
    
- 书写位置：head标签里面，title标签下方添加style双标签，style标签里面书写CSS代码。

```html
<title>CSS初体验</title>
	<style>
	 /*选择器{}样式*/
	 p {
		 /*CSS属性*/	 
		 color:red;
		 }
	 
	</style> 
	
	
<p>体验CSS</p>
```

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>初始CSS</title>
        <style>
            p {
    		        /* 颜色调整 */
    		        /* 属性名与属性值成对出现-》键值对 */
                color: red;
                /* 字体变大 */
                font-size: 30px;
            }
        </style>
    </head>
    <body>
        <p>体验CSS</p>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:8caebbbc-bb85-4a6b-8fb4-5dc0bb6d5ec9:image.png)
    
    ![image.png](attachment:953fcf57-21b4-430f-87b1-cbd04a1fba05:image.png)
    

## CSS引入方式

- 内部样式表：学习使用
    - CSS代码写在style标签中
- 外部样式表：开发使用
    - CSS代码写在单独的CSS文件中（**.css**）
    - 在HTML使用Link标签引入
        
        ```html
        **<link rel="stylesheet" href="./my.css">**
        ```
        
- 行内样式：配合JavaScript使用
    - CSS写在标签style属性值里
        
        ```html
        **<div style="color:red; font-size:20px">这是div标签</div>**
        ```
        

- 代码演示
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <!-- link引入外部样式表 -->
        <link rel="stylesheet" href="./my.css">
    </head>
    <body>
        <p>这是一个p标签</p>
        <!-- 行内样式，配合JS使用 -->
        <div style="color: blue; font-size: 30px;">这是一个div标签</div>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:ec3581c3-8444-4ccb-abba-5987585ee1cf:image.png)
    

<aside>
💡

**修改样式后注意保存！**

</aside>

## 选择器

作用：查找标签，设置样式

**基础选择器**

- 标签选择器
    - 使用**标签名**作为选择器 → 选中**同名标签**设置**相同的格式**
        - 例如：p,h1,div,a,img ……
        - **无法差异化同名标签的样式**
    - 代码演示
        
        ```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>标签选择器</title>
            <style>
                p {
                    color: red;
                }
            </style>
        </head>
        <body>
            <p>这是一个P标签</p>
            <p>这也是一个p标签</p>
            
        </body>
        </html>
        ```
        
        ![image.png](attachment:83c1d213-a5e5-4d93-ad35-eba28ec6fd50:image.png)
        
- 类选择器
    
    作用：查找标签，**差异化**设置标签的显示效果
    
    步骤：
    
    - 定义类选择器 → **.类名**
    - 使用类选择器 → 标签添加**class=“类名”**
    
    ```html
    <style>
    	.red {
    			color: red;
    			 }
    </style>
    
    <div class="red">这是div标签</div>
    ```
    
    - 代码演示
        
        ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>类选择器</title>
            <style>
                .red {
                    color: red;
                }
        
                .size {
                    font-size: 30px;
                }
            </style>
        </head>
        <body>
            <p class="red">111111</p>
            <div class="red">222222</div>
            <div class="size">444444</div>
            <p class="red size">333333</p>
        </body>
        </html>
        ```
        
        ![image.png](attachment:a2e037af-344c-44c1-9c44-906cc953025a:image.png)
        
    
    <aside>
    💡
    
    类名自定义，**不要用纯数字或中文**，尽量用英文命名
    
    一个标签可以使用**多个**类名，用**空格**隔开
    
    一个类选择器可以给**多个标签**使用
    
    开发习惯：类名**见名知意**，多个单词可以用-链接，例如：**news-hd**
    
    </aside>
    
- id选择器
    
    作用：查找标签，**差异化**设置标签的显示效果
    
    场景：id选择器一般**配合JS使用**，很少用来设置CSS样式
    
    步骤：
    
    - 定义id选择器 → #id名
    - 使用id选择器 → 标签添加 id = “id名”
    
    ```html
    <style>
    	#red {
    			color: red;
    			 }
    </style>
    
    <div id="red">这是div标签</div>
    ```
    
    <aside>
    💡
    
    **同一个id选择器在一个页面只能使用一次**
    
    </aside>
    
    代码演示：
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>id选择器</title>
        <style>
            #red {
                color: red;
            }
        </style>
    </head>
    <body>
        <!-- id选择器的使用-->
        <div id="red">这是一个div标签</div>
        
    </body>
    </html>
    ```
    
    ![image.png](attachment:cbf212d2-e30c-4346-99bc-a4812f7d97a5:image.png)
    
- 通配符选择器
    
    **作用**：查找页面**所有标签，设置相同样式。**
    
    **通配符选择器**：***，不需要调用，**浏览器**自动**查找页面**所有**标签，设置相同的样式。
    
    ```html
    * {
    	color: red;
    }
    ```
    
    **使用场景：**
    
    在项目初期，用于清除默认样式，例如：每一行之间默认间隔
    
    ![image.png](attachment:8c4f1c61-7bae-42d6-95df-670cebbc6c03:image.png)
    
    **代码演示：**
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <style>
            * {
                color:blue;
            }
        </style>
    </head>
    <body>
        <div>这是一个div标签</div>
        <p>这是一个p标签</p>
    </body>
    </html>
    ```
    
    ![image.png](attachment:1de049b3-9ff2-4968-bc46-94c12462375c:image.png)
    

## 画盒子

**目标：使用合适的选择器画盒子**

**代码演示：**

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>画盒子</title>
    <style>
        .red {
            width: 100px;
            height: 100px;
            background-color: red;
        }

        .orange {
            width: 200px;
            height: 200px;
            background-color: orange;
        }
    </style>
</head>
<body>
    <div class="red">div1</div>
    <div class="orange">div2</div>
    
</body>
</html>
```

![image.png](attachment:b15f070f-420a-482b-baae-b51d059a9009:image.png)

## 文字控制属性
