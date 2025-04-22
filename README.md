## Hi there 👋
开始
基础

1.<!DOCTYPE html>
(1). 作用：告知浏览器该页面文件的文档类型，指示web浏览器使用哪个HTML版本编写页面。（2）.位置：<!DOCTYPE> 声明必须是 HTML 文档的第一行，位于 <html> 标签之前。 (3). <!DOCTYPE> 声明对大小写不敏感。 (4). <!DOCTYPE> 声明没有结束标签。
2. <html lang="en">...</html>
(1). 此元素可告知浏览器其自身是一个 HTML 文档。 (2). <html> 与 </html> 标签限定了文档的开始点和结束点，在它们之间是文档的头部和主体。文档的头部由 <head> 标签定义，而主体由 <body> 标签定义。 (3). lang 属性（语言属性）：当搜索引擎或者浏览器拿到语言属性后，有可能做一些针对指定语言的辅助操作，‘en’表示英文。
3. 标签属性
(1). 标签可以拥有零个或多个标签属性，注意：标签属性与标签名称、标签属性与标签属性之间需用一个空格隔开。 (2). 标签属性可以赋予标签更多的信息，标签属性通常是以 key="value" 即 名称="值" 的形式出现。 (3). 常见的标签属性有：class、id、style、lang、src 等。
4. 文档的头部<head>...</head>
(1). head 元素定义文档的头部，我们通常在这里引用样式表、提供元信息等。 (2). 文档的头部中的<title>...</title>定义文档的标题，在网页上体现为网页标签的标题。 (3). 一个 <head> 元素必须包含且只能包含一个 <title> 元素。
元信息：又叫元数据，就是描述数据的数据。这里主要指文档的概要信息。
5. 文档的主体<body>...</body>
（1）.body元素定义文档的主体，包含文档的所有内容（比如文本、超链接、图像、表格和列表等等）。
6.每个编译语言都有注释，html也不例外，在HTML中我们使用<!-- -->标签来表示注释：

网页中显示的内容如下：

注释标签用于在源代码中插入注释。注释不会显示在浏览器网页中的。


第二
简单使用其他<>
<img> 为例，来演示如何使用 MDN 文档。
1. 搜索
打开上面的链接，我们会看到这样的一个页面：
（1）在标注 1 的地方，我们可以切换网页显示的语言。 （2）在标注 2 的地方，我们输入 img 进行搜索。
因为我们要搜索的是 img 标签（html tag），所以点击第二条纪录：

1. 阅读文档
打开后看到如下界面，通常一个 HTML 标签（html tag）的文档都会包含该标签的概述、标签属性的介绍、应用的例子和浏览器兼容性等内容。

翻到介绍标签属性的位置，可以看到文档中介绍了img 标签的各个标签属性的作用，下图中被框出来的 title 、 align 、 alt等都是 img 标签的属性。

在页面最开始的地方，可以看到使用的示例，到这里大家应该对如何使用img标签有了一定的了解：


<p> <h1> <h2>... <strong>
图片<img>
<img>标签，我们已经见过它很多次了，它的使用方法如下：显示效果：

点击播放上述代码：
代码演示
在标签属性src中写入图片的 相对路径 或 绝对路径 就可以啦。
图片标签还有个 alt 属性，这个属性定义了描述图像的替换文本。如果图像的 URL 是错误的，该图像不在 支持的格式 列表中，或者如果图像还没有被下载，用户将看到这里的替换文本。
alt 的效果是这样的：

除了静态的 jpg、jpeg、png 之类的图片，我们还可以用 img 标签向网页中插入 gif 动图哦：

网页显示效果：

超链接<a>
<a>标签是内联标签，用户点击后，浏览器会跳转到指定的网址。下面就是一个典型的链接。
链接代码：
显示效果：
点击播放：
代码演示
浏览器显示“优课达”，文字下面默认会有下划线，表示这是一个链接。用户点击后，浏览器跳转到 href 属性指定的网址。
<a>标签内部不仅可以放置文字，也可以放置其他元素，比如段落、图像、多媒体等等。比如：
链接代码：
显示效果：
点击播放：
代码演示
下面我们来了解一下链接标签中比较重要的属性：
链接标签的属性
href
href 属性给出链接指向的网址。它的值应该是一个 URL 或者锚点。
URL：统一资源定位符（英语：Uniform Resource Locator，缩写：URL；或称统一资源定位器、定位地址、URL 地址，俗称网页地址或简称网址）是因特网上标准的资源的地址（Address）。
title
title 属性给出链接的说明信息。鼠标悬停在链接上方时，浏览器会将这个属性的值，以提示块的形式显示出来。 title 属性：
target
target 属性指定如何展示打开的链接。
target 属性的值也可以是“_self”、“_blank”、“_parent”、“_top”四个关键字之一。
1. 当它为_self 时表示在当前页面打开，target 默认为“_self”。
显示效果：优课达
1. 当它为_blank 时表示在新页面打开。
显示效果：优课达
点击播放上述代码：
代码演示
target 属性的值分别是“_self”、“_blank”时打开链接的表现：
<ol>有序 <ul>无序
除了我们之前在文章中用到的 **标题标签** <h1>~<h6> 、 段落标签<p> 、 内联标签<span> <strong> 、 图片标签<img>(也是内联标签)、 链接标签<a>(也是内联标签)外，列表标签也是很常用的文本标签。
HTML提供了无序列表标签<ul>和有序列表标签<ol>供我们选择，这里我们选择无序列表标签<ul>，列表的每一项都用标签<li>表示，点击播放：
代码演示

显示效果：
● 列出今天要做的事情
● 每天结束填写回顾和反思
● 计划第二天的内容
我们可以看到，每个列表项<li>前面有个实心小圆点，这是无序列表的符号，当不需要考虑列表项的顺序时，我们常常采用无序列表标签<ul>。
如果想要显示有排序的列表项，我们会用<ol>标签，它的列表符号会是数字或者字母等，点击播放：
代码演示

显示效果：
1. 列出今天要做的事情
2. 每天结束填写回顾和反思
3. 计划第二天的内容
<注册表格>
在浏览 Web 时，用户的交互主要是通过点击 链接 来浏览网页。 但有时我们也需要用户通过 输入 来提供一些信息。比如：
● 注册并登录网站
● 输入个人信息（姓名，地址，信用卡详细信息……）
● 过滤内容（使用下拉菜单，复选框……）
● 进行搜索
● 上传文件
● …
为了满足这些需求，HTML 提供了交互式 表单控件 ：
● 文本输入（一行或多行）
● 单选按钮
● 复选框
● 下拉菜单
● 上传小部件
● 提交按钮
form 标签
现在让我们来完成下面这个表单的开发
可以看到，在这个注册表单里都是输入框、按钮等表单元素，对于这些表单控件，我们需要用一个块状元素<form>把它们包起来，属于同一个表单的表单控件要包含在同一个块状元素<form>里。
这个标签有两个属性需要我们了解，action和method：
1. action：一个处理此表单信息的程序所在的 URL，所述表格信息将在表单提交时被发送到定义的地址；
2. method：它的值可以是 GET 或 POST，用来规定 如何 发送表单信息；
通常，表单信息被发送到 服务器 。如何处理这些数据不是我们本次课的内容，我们以后会再讲到。
现在让我们先写下一个<form>标签，在网页上定义一个表单区域：
<!-- <form>是块状标签，要注意：<form>标签不能嵌套<form>标签 -->
<form action="">
  <!-- 这里会有一些表单控件 -->
</form>

昵称输入框
<!-- action=""则表单信息将提交到当前页面 -->
<form action="">
  <input type="text" />
</form>
显示效果：
特别注意：需要我们特别关注的是，input不但是一个内联元素，还是一个只有开始标签，没有结束标签的内联元素，我们可以认为它是一个“自闭”元素。你还记得别的自闭元素吗？
1. 占位文本 “placeholder”
我们可以看到，注册表单（上图）中的昵称输入框里有“昵称”两个字，而我们的单行文本输入框中并没有任何文字，这个文字在点击输入框并输入内容后会消失，这是 占位文本，通常用来 提示 用户需要输入什么。可以通过标签属性 “placeholder” 来实现的。
<input type="text" placeholder="昵称" />
显示效果： 
2. 输入框名字 “name”
为了区别于其他的<input>，我们需要给昵称输入框加上标签属性name，作为<input>的名字，在提交表单数据时就不会和其他<input>搞混了：
<input type="text" placeholder="昵称" name="nick" />
显示效果：
3. 输入框的值 “value”
如果希望在输入框中预填写用户的昵称，可以用标签属性value：
<input type="text" placeholder="昵称" name="nick" value="小明" />
显示效果： 
4. 不可修改的输入框 “readonly”和“disabled”
在一些特殊情况中，我们会给用户分配昵称，这个时候并不希望用户可以自行修改，我们可以这么做：
<input type="text" placeholder="昵称" name="nick" value="小明" readonly />
显示效果： 
把输入框变成 只读 输入框！这样用户就不能自己修改预填写的内容啦。
除了用”readonly”这个属性，我们还可以用”disabled”，这个属性也能使用户无法更改输入框中的内容。
<input type="text" placeholder="昵称" name="nick" value="小明" disabled />
显示效果： 
但是这两个是有一定区别的：
属性	disabled	readonly
对象	所有表单元素	input 和 textarea
作用	使文本框不能输入，当表单以 POST 或 GET 的方式提交时，使用了 disabled 的元素的值不会被传递出去	仅使文本框不能输入
外观 *	使文本框变灰	外观没有变化
外观 * ：在不同浏览器中输入框的外观可能会有区别，因此“readonly”和“disabled” 这两种输入框在外观上的差别可能与上表所述有所不同。

 
多行输入框（个性签名）
这里我们会用到textarea标签来写多行输入框。
<!-- name属性表示表单元素的名称，placeholder属性表示表单元素的占位文本 -->
<textarea
  name="sign"
  rows="5"
  cols="30"
  placeholder="请输入个性签名"
></textarea>
显示效果： 
点击播放上述代码：
其中rows和cols分别表示行数（高度）和文本域的可视宽度： rows：行数（高度）； cols：文本域的可视宽度；
这两个属性可写可不写，<textarea></textarea>就能表示一个多行输入框，显示效果： 
在多行文本框右下角我们可以看到一排斜线：在斜线处按住鼠标左键拖动，可以改变输入框的大小。
密码输入框
密码输入框和昵称输入框有点区别，用户输入的内容将会以 黑圆点 的形式显示。
如何做到输入内容不直接显示呢？ 非常简单，我们只需要把表单标签<input>中的标签属性type="text"改成type="password"就可以啦：
<!-- type属性表示表单元素的类型，name属性表示表单元素的名称，placeholder属性表示表单元素的占位文本 -->
<input type="password" name="password" placeholder="密码" />
显示效果如下，你可以在下面的输入框中输入内容试一试： 
点击播放上述代码：

现在我们把下图这个表单中的个性签名输入框和密码输入框加上，点击播放：




<单选框和复选框>
性别单选题（单选框）
在这里我们只考虑了男女两种性别，并默认用户只有一种性别。 就像做单选题一样，用户只能选择男性或者女性。
这里我们得使用 单选框：
<!-- type属性表示表单元素的类型，name属性表示表单元素的名称，value属性表示表单元素的值 -->
<input type="radio" name="gender" value="male" />
<input type="radio" name="gender" value="female" />
显示效果：  
所谓单选框，其实只是把控件类型ttype="text"改成了type="radio"。 大部分 表单元素都是通过改变标签属性type的值来实现的。
* 属于同一道“单选题”的每个单选按钮，应该拥有 相同 的name属性值。
我们用 value=“male” 表示男性，用 value=“female” 表示女性，但是大家会发现，在上面的网页显示效果中并没有这两个单词出现，其实，这两个单词是表单数据提交时提交的内容。
那么我们如何把选项的内容写到网页上呢？很简单，直接在input标签后加内容就可以啦：
<input type="radio" name="gender" value="male" />男
<input type="radio" name="gender" value="female" />女
显示效果：  男  女
现在，当用户点击文字前面的小圆点时，就会选中对应的性别啦，点击试试吧。
但是，这样点击的范围有点小，如果点击文字也能选中对应的性别就更好了。 为了达到这个目的，我们常常会把单选框和标签<label>配合使用：
<label> <input type="radio" name="gender" value="male" />男 </label>
<label> <input type="radio" name="gender" value="female" />女 </label>
显示效果：  男  女
点击播放上述代码：
代码演示
现在点击文字也能选中对应的性别！试试看吧！
另一种写法：
<input id="male" type="radio" name="gender" value="male" />
<label for="male">男</label>
<input id="female" type="radio" name="gender" value="female" />
<label for="female">女</label>
我们给单选框<input>加了一个属性id="male"，给<label>标签也加了一个属性for="male"。这样，两者之间就产生了一一对应的关系。 显示效果：  男
 女 点击播放上述代码：
代码演示
兴趣多选题（复选框）
用户可能对很多领域感兴趣，所以在兴趣的选择上我们要用复选框。
复选框的使用就像一道多选题，用户可以选择多个选项。除此之外，复选框和单选框很像，它的类型是checkbox：
<input type="checkbox" />
显示效果： 
点击播放上述代码：
代码演示
你会在页面上看到一个小方框，点击它，可以看到它被选中了，再次点击，选中会被取消。
为了写好我们的兴趣复选框，我们需要在上面这个简单的复选框的基础上，给它们加上文字（配合<label>标签）、name 属性和 value 值：
<label> <input type="checkbox" name="interest" value="coding" />编程 </label>
<label> <input type="checkbox" name="interest" value="other" />其他 </label>
显示效果：  编程  其他
点击播放上述代码：
代码演示
* 属于同一道“多选题”的每个复选框元素，应该拥有 相同 的name属性值。
需要注意的是：复选框是只有 2 种状态的表单控件：已选中或未选中。在只有一个复选框的情况下，它允许用户对某事说“是”或“否”，比如同意或不同意某个条款。而只有一个单选框的情况下，用户一旦选择了这个单选框，就不能再取消选择了，除非他刷新了网页～
现在我们把下图这个表单中的性别输入框和兴趣多选框加上（样式可能和下面这个表单有些不同，大家先不用纠结这一点，样式的问题等我们学习样式之后再讨论），点击播放：

因为男女是同一选择中的so name 相同 
拓展多选

 <select>和<option>，选项菜单。

每个选项用<option>标签表示，一组选项用<select>包裹：
<select name="career">
  <option value="default">请选择职业</option>
  <option value="staff">公司职员</option>
  <option value="freelancer">自由职业者</option>
  <option value="student">学生</option>
  <option value="other">其他</option>
</select>
显示效果：   
点击播放上述代码：

需要注意的是，这是一个单选菜单，如果用户选择了“学生”，那么提交的数据将会是：career:"student"
发现了吗？提交的内容并不是“学生”，而是<option>标签的标签属性value的值。所以每个 option 的 value 值要互不相同。
如果我们想要的是一个多选菜单，该怎么办呢？
很简单，给<select>标签添加 multiple 属性，就可以通过按住 Ctrl（或 ⌘）并单击选项来选中多个选项啦：
<select name="career" multiple>
  <option value="default">请选择职业</option>
  <option value="staff">公司职员</option>
  <option value="freelancer">自由职业者</option>
  <option value="student">学生</option>
  <option value="other">其他</option>
</select>
显示效果：   

点击试试看，这次可以选中多个选项了。
<button>注册</button>
显示效果： 注册
点击播放上述代码：
代码演示
因为<button>标签有闭合标签，在开始标签和结束标签之间，我们可以放上文字、图片、图标等等。
这个按钮放在 form 中会在点击的时候自动提交表单数据，但是在 button 提交表单数据这一点上是有浏览器兼容性问题的，一般还是需要加上 type=“submit”来确保数据的提交：
<button type="submit">注册</button>
显示效果： 注册
点击播放上述代码：
代码演示
现在我们把下图这个表单中的职业选择菜单加上，点击播放：
代码演示
到这里，我们就完成了一个简单的注册表单。
完整的注册表单：
<form action="">
  <input type="text" name="name" placeholder="请输入昵称" />
  <textarea
    name="sign"
    rows="5"
    cols="30"
    placeholder="请输入个性签名"
  ></textarea>
  <input name="password" type="password" placeholder="请输入密码" />

  <label> <input type="radio" name="gender" value="male" />男 </label>
  <label> <input type="radio" name="gender" value="female" />女 </label>

  <label> <input type="checkbox" name="interest" value="coding" />编程 </label>
  <label> <input type="checkbox" name="interest" value="other" />其他 </label>

  <select name="career">
    <option value="default">请选择职业</option>
    <option value="staff">公司职员</option>
    <option value="freelancer">自由职业者</option>
    <option value="student">学生</option>
    <option value="other">其他</option>
  </select>

  <button type="submit">注册</button>
</form>

小总结
 

文字格式
5.1HTML 内部添加样式
1 在标签中添加声明
声明的关键字是style后接等号（=）再接引号（""），即style=""
具体声明如下：
<input type="text" placeholder="手机号码" style="">
● 声明位置不分先后
<input type="text" style="" placeholder="手机号码">
<!-- 或者 -->
<input style="" type="text" placeholder="手机号码">
以上两种方式都正确
● 与其他关键字之间用空格隔开
关键字和关键字之间要用空格隔开，比如type和placeholder之间会加一个空格
<input type="text" placeholder="手机号码" style="">
注意：关键字和标签名之间也要用空格隔开，比如下面这种写法就是错误的
<pstyle=""></p>
2 在引号之间添加样式
<p style="font-size:14px;color:white"></p>
这段代码的意思就是：设置p标签中的字体大小为14px，颜色为白色。
CSS样式我们在后面会学到，这段代码不理解也不要紧。
5.2 字体大小/字体粗细
在css中，样式是由属性和值组成中间用冒号（:）隔开，用分号（;）收尾，其中属性可以理解为身高、体重，值可以理解为 1.8 米、60kg，在现实生活中我们用这样一对组合来描述人或者物，在 CSS 中，我们用这样一对组合来描述文字的粗细、大小、颜色等等。

字体大小
设置格式为：font-size:36px;
font-size --> 字体的大小 36px --> 字体大小的尺寸
注意：
你可能会在以后的代码中看到这样的现象，style = "font-size: 12px; font-weight:bold"。可以看到，bold 后面没有分号;，这是因为这一组属性后面再没有其他的属性了，所以可以把结尾的分号;省略，但是这样的写法允许，但不规范。
核心代码如下：
<!-- 设置字体的大小为12px -->
<p style="font-size: 12px;">
  一个轻量级和模块化的前端框架，用于开发快速和强大的web接口。
</p>
<!-- 设置字体的大小为24px -->
<p style="font-size: 24px;">
  一个轻量级和模块化的前端框架，用于开发快速和强大的web接口。
</p>
点击下方的播放按钮查看代码演示

字体加粗
设置格式：font-weight:100;
设置文字粗细的时候，其值可以是 100，200，300，400，500，600，700，800，900 中的任何一个,或者可以用英文代替，normal（正常粗细），lighter(细)，bold（粗），bolder（更粗）
下面我们来看看使用不同的值去设置字体粗细的效果
font-weight:200;
优课达
font-weight:lighter;
优课达
font-weight:400;
优课达
font-weight:normal;
优课达
font-weight:700;
优课达
font-weight:bold;
优课达
核心代码如下：
<p style="font-weight: 200;">优课达--学的比别人好一点～</p>
<p style="font-weight: lighter;">优课达--学的比别人好一点～</p>
<p style="font-weight: 400;">优课达--学的比别人好一点～</p>
<p style="font-weight: normal;">优课达--学的比别人好一点～</p>
<p style="font-weight: 700;">优课达--学的比别人好一点～</p>
<p style="font-weight: bold;">优课达--学的比别人好一点～</p>
点击下方的播放按钮查看代码演示




5.3 字体颜色/文字对齐方式
颜色
颜色是页面中不可或缺的属性，在背景、文字中应用非常广泛，颜色的值的设置方式分为四种：
1. 英文字母形式
● color: black;
 
● color: blue;
 
● color: red;
2. 十六进制颜色 十六进制颜色由#开头，后面跟三个数字，每个数字的范围为 00 ～ FF，每个数字代表一种颜色，最终的颜色由这三种颜色调和而成； 这个颜色一般由设计师给我们，或者可以用吸色工具去获取。
● color: #DAE8FC;
 
● color: #D5E8D4;
3. rgb 形式 rgb 形式和十六进制的原理相同，其最终的颜色由三种颜色的深浅决定，即 r(red)，g(green)，b(blue)，每种颜色的范围为 0 ～ 255，代表这每种颜色的深浅，值越大越深；同样的，我们不必去深入研究它，设计师给我们什么，我们就用什么。
● color: rgb(253, 217, 106);
4. rgba 形式 rgba 形式相比 rgb 形式，多了一个 a，这里的 a 代表的是 Alpha(透明度)，a 的值在 0 ～ 1 之间，为了简化书写，也可以直接省略 0，写成.4，等同于 0.4。
● color: rgba(253, 217, 106,1.0);
 
● color: rgba(253, 217, 106,0.3);
注意：以上四种表达方式：
1. 多数情况下建议使用十六进制表达方式；
2. 调试的时候可以用英文字母形式，初期的调试就是随便设置一个颜色，查看区块是否存在，区块大小等，在盒模型中我们会遇到；
3. 如果要设置文字透明度或者背景透明度，就要用到rgba形式，在第八章我们会遇到。
下面我们来使用字体颜色来实现下图效果：
UIzards
Senior UX Designer
Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quom placerat facer possim assum. Typi non habent claritatem insitam; est usus legentis in iis qui faorum claritatem. Investigationes demonstraverunt lectores legere me lius quod ii legunt saepius.
核心代码如下：
<h3 style="color:#ff9a9e;font-weight:700;font-size: 24px;">UIzards</h3>
<h4 style="font-size: 16px;color: #474d5d;font-weight: 400;">
  Senior UX Designer
</h4>
<p style="font-size: 14px;color:#84868d;">
  Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet
  doming id quom placerat facer possim assum. Typi non habent claritatem
  insitam; est usus legentis in iis qui faorum claritatem. Investigationes
  demonstraverunt lectores legere me lius quod ii legunt saepius.
</p>
点击下方的播放按钮播放代码演示
代码演示
文字居中/居左/居右
在学习这一节的文字对齐方式的时候，大家可以结合 word 这个办公软件的文字对齐方式去理解，原理是一样的。具体对齐方式效果如下图所示：
文字左对齐
文字对齐方式左对齐文字对齐方式左对齐文字对齐方式左对齐文字对齐方式左对齐文字对齐方式左对齐
文字右对齐
文字对齐方式右对齐文字对齐方式右对齐文字对齐方式右对齐文字对齐方式右对齐文字对齐方式右对齐
文字居中对齐
文字对齐方式居中对齐文字对齐方式居中对齐文字对齐方式居中对齐文字对齐方式居中对齐
设置文字对齐的格式如下：
● text-align: center; 文字居中对齐
● text-align: left; 文字左对齐
● text-align: right; 文字右对齐

 
行高
首先来解释一下行高，我们先来看一张图：

图中虚线框的高度就是我们之前学过的font-size(字体大小)，以图中的行高为例，20px的行高除去文字大小12px后，将剩下的8px均分为两部分，分别填充在文字上下；
两行文字之间的距离就是由第一行文字下面的4px加第二行文字上面的4px形成一个8px的间距，因此行高的大小决定了文字行与行之间距离的大小。
行高的设置格式：line-height: 30px;
在实际应用中，行高的作用主要有两个：
第一个作用：改变段落中行与行之间的距离
段落中默认是有行高的，但是这个默认的行高未必能满足我们的需求，因此我们就需要改变行高来实现我们需要的效果；
下面我们来看一个案例，第一个p标签内的行高为默认高度，第二个p标签的行高为32px，下图是结果：
We understand every aspect of project and we put a great amount of time in understanding the project.
We understand every aspect of project and we put a great amount of time in understanding the project.
核心代码如下：
<p>
  We understand every aspect of project and we put a great amount of time in
  understanding the project.
</p>

<p style="line-height:32px;">
  We understand every aspect of project and we put a great amount of time in
  understanding the project.
</p>
点击下方的播放按钮查看代码演示
代码演示
第二个作用：使文字上下居中
从下图可以看出，随着行高的变化，文字的位置也在不断变化，当行高和矩形的高度一样的时候，文字在矩形中上下居中。
例如：文字外面的矩形高度为 80px，要想让文字在矩形中上下居中，就要设置文字的行高为 80px

如下图所示，我们可以使用做一个文字居中的按钮：
提交
核心代码如下： 为了美观，背景颜色和圆角我们在 index.css 中写出，后面我们会学到，这里不用纠结
<button
  style="width: 120px;height:50px;text-align: center;line-height:50px;color:white;font-size: 18px;"
>
  提交
</button>
点击下方的播放按钮查看代码演示
代码演示
字间距
字间距就是文字之间的间距，但是中文和英文的字间距是不一样的
● 英文的字间距是每个字母之间的距离，单词和单词之间的距离不属于字间距
● 中文是每个汉字之间的距离
设置字间距的格式为：letter-spacing: 30px;
代码演示
字体
字体的概念我们在生活中肯定接触了很多，比如说宋体，隶书，黑体，草书等等，当然还有很多外国字体，比如微软雅黑。
字体了解了，那么我们如何去设置字体呢？其实设置字体的方式很简单，关键字+值即可，例如：
font-family: sans-serif;
我们设置的字体能否被应用在页面上取决于使用者的电脑有没有安装这个字体，所以网页中会使用一些常见的字体，使得自己的网站兼容性更好。
当然了，有的网站比较个性化，喜欢用一些个性化的字体，所以他们会多设置几个字体，比如：
font-family: 'Goudy Bookletter 1911', sans-serif, 'Gill Sans Extrabold';
这段代码怎么去理解呢？页面加载以后会先去找代码中设置的字体，这里有三个备选的字体，浏览器会按顺序加载：首先看看"Goudy Bookletter 1911"字体在电脑上是否安装；如果没有安装，就去看第二个字体；如果还没有，就去看第三个字体是否已经安装；如果都没有安装，那么就只能用默认的微软字体，这个字体是所有电脑默认会安装的。
字体写法有一些注意事项：
● 多个字体之间用英文逗号（,）隔开
● 字体名称中间有空格的时候，要加引号，单引号和双引号都行："Times News Roman"
● 中文字体名称要用引号，单引号和双引号都行："宋体"

1.1 HTML5/CSS3介绍
认识HTML5
HTML5简而言之就是HTML的升级版，在之前的基础上添加了更多的功能，丰富了一些属性，让页面制作更加多元化，相比之前的HTML而言，HTML5功能更强大、页面效果更绚丽，下面我们观看几个案例来感受一下HTML5制作出来的页面效果：
语义化标签
其实在我们学习HTML的时候，就已经接触到了语义，比如我们之前使用的：
● <p></p>标签代表段落
● <h1></h1>标签代表一级标题
● <li></li>标签代表列表
这就是语义化标签，即标签的名字赋予标签的意义和作用。
但是div代表什么呢？显然是无法根据div这个标签名判断div在页面中的位置，比如下面这个页面，它的页面结构非常清晰。

下面用我们常用的布局方法来将上面这张图转化成代码，代码如下：
<div></div>
<div></div>
<div></div>
大家有没有注意到一个问题，本来清晰的页面结构，写成代码以后，仅靠阅读代码，我们无法在脑海中形成之前的页面结构。
语义化标签就是用来解决这个问题的，对应上面每一个区块，在HTML5中都有对应的语义化标签，下面我们用语义化标签来改造一下上面这段代码：
<!-- 头部 -->
<header></header>
<!-- 主体 -->
<main></main>
<!-- 底部 -->
<footer></footer>
仅通过阅读代码，就可以确定页面结构，这就是语义化标签的意义所在。
常用的语义化标签
常用的语义化标签不止上面三个，下面这个布局所涉及的语义化标签基本涵盖了我们常用的所有语义化标签：

对应的HTML代码如下：
<!-- 头部 -->
<header>header</header>
<!-- 主体 -->
<main>
    <!-- 导航 -->
    <nav>nav</nav>
    <!-- 区块 -->
    <section>section</section>
    <section>section</section>
</main>
<!-- 侧边栏 -->
<aside></aside>
<!-- 底部 -->
<footer></footer>
语义化标签的使用场景
下面我们以“淘宝网”首页为例，来理解语义化标签的使用场景。
<header></header>——头部
header标签用于展示介绍性内容，通常包含一组介绍性的或者是辅助导航的实用元素。
例如淘宝页面中的顶部：
<main></main>——主体
main标签通常是页面的主体内容区域。
例如淘宝页面中header以下footer以上的所有内容:
但是在实际应用中，需要根据具体情况去分析，只要是某个区块的主体就可以用main标签，暂时我们不用纠结，只记住上面这一种即可。
<footer></footer>——底部
footer表示页面页脚部分的版权数据、与文档相关的链接、责任声明等信息。
网页中最常见的footer就是页面最底部的一些额外信息：
淘宝的页面footer内容比较多，一般网站的footer信息不会很多。
<nav></nav>——导航
nav:定义文档或者页面的导航
比如网页中的商品类别导航：
<aside></aside>——侧边栏
aside:定义页面的侧边栏内容
如淘宝的侧边栏：
<section></section>——区域块
section:定义文档中的节，区域块，section更像接近div的语义，就是在页面中开辟一块空间。
比如下面这个页面中，我们首先要将页面分成左右两部分，这里就可以用section去区分：
基本上，语义化标签的使用场景就是这么多，还有一些更深入的使用场景，我们暂时先不用去了解，只要知道常用的一些使用场景即可。
CSS3
CSS3和HTML5的关系你可以理解为CSS和HTML之间的关系，由于CSS3修改内容较多，我们在后续章节会展开讲，在本章不做多于赘述。
2.1 CSS伪元素--::after/::before
网页中我们经常会在页面的头部见到下图中的布局：

我们的做法是这样的，核心代码如下：
<span class="icon"></span><span class="words">主页</span>
.icon {
    display: inline-block;
    width: 24px;
    height: 24px;
    background: url(https://qgt-document.oss-cn-beijing.aliyuncs.com/P3-2-HTML-CSS/1.2/source/first-page.png) no-repeat center;
    background-size: contain;
    vertical-align: top;
    margin-right: 8px;
}

.words {
    font-size: 18px;
    line-height: 24px;
}
我们来通过代码演示来看一下最终的效果：
代码演示
其实我们有一种更好的方法来完成上述案例，即伪元素。
伪元素就是利用css代码在标签内部的前面，或者后面添加一个行内元素，这个行内元素你可以理解为span。
下面我们来认识一下伪元素的写法：
/* before */
选择器::before{
  /* 使用空白符号占位 */
  content: '';
}

/* after */
选择器::after{
  /* 使用空白符号占位 */
  content: '';
}
接下来我们来使用伪元素实现开头的案例：
1. 去除HTML代码中类名为icon的span标签
<span>主页</span>
1. 修改CSS代码
/* 在span之前添加行内元素 */
span::before {
  content: '';
  /* 将添加的行内元素定位，并设置大小、背景 */
    position: absolute;
    left: 0px;
    width: 24px;
    height: 24px;
    background: url(https://qgt-document.oss-cn-beijing.aliyuncs.com/P3-2-HTML-CSS/1.2/source/first-page.png) no-repeat center;
    background-size: contain;
}
最后我们通过代码演示来看一下最终的效果：
代码演示
上述案例中我们将添加的行内元素做了定位处理，其实还可以将添加的行内元素转换成块元素（block）或者行内块元素（inline-block）来实现我们需要的效果。
下面我们要用display来做一个案例，在很多网页中的轮播图中，我们可以看到这样的用来切换图片的小圆点，如下图所示：

将这里的小圆点放大一点后，如下图：

这个案例就不用去对比常规写法和伪元素写法了，我们直接用伪元素来完成上图效果，核心代码在下面贴出：
<div class="circle"></div>
.circle {
    box-sizing: border-box;
    width: 200px;
    height: 200px;
    margin: 20px auto;
    border-radius: 50%;
    background: #9995A5;
    /* 使用padding让子元素居中 */
    padding: 30px;
    border: 10px solid #8E8A97;
}

.circle::before{
   content: '';
  /* 将添加的行内元素转成块元素 */
    display: block;
    width: 120px;
    height: 120px;
    border-radius: 50%;
    background: #666278;
}
代码演示
在之前的例子中我们都用的是::before，没有介绍过::after，其实::after和::before是一样的，当我们需要第二个行内元素的时候，就需要用after
2.2 CSS伪类--清除浮动
浮动带来的问题
我们先来看一个页面，如下图：
son-one
son-two
son-three
要完成这个案例，最好的办法就是子元素设置高度，父元素的高度由子元素撑起来，使父元素的高度可以自适应，核心代码如下：
<div class="father-one">
    <div class="son-one">son-one</div>
    <div class="son-two">son-two</div>
    <div class="son-three">son-three</div>
</div>
.father-one {
    border: 2px solid #8E8A97;
    text-align: center;
}

.son-one {
    line-height: 50px;
    background-color: #00FFFF;
}

.son-two {
    line-height: 100px;
    background-color: #00BFFF;
}

.son-three {
    line-height: 50px;
    background-color: #00FFFF;
}
代码演示
影响父元素兄弟元素的布局
下面我们给.father-one后面添加一个兄弟元素，然后让.father-one里面的所有子元素都浮动，看一下会出现什么现象：
核心代码如下（代码中省略了部分已有代码）：
<!-- 添加father-one的兄弟元素 -->
<div class="father-two"></div>
.son-one{
  /* 浮动后的元素宽度默认和它内容的宽度一致，即和文字的宽度一致。
  这里为了美观，设置一个自定义宽度*/
  width:33.3%;
  float:left;
}

.son-two{
  width:33.3%;
  float:left;
}

.son-three{
  width:33.3%;
  float:left;
}

.father-two{
  height: 150px;
  background-color: #CACACA;
}
最终得到下图所示的页面效果：
son-one
son-two
son-three
观察上图，会发现类名为father-two的div的一部分内容会跑到father-one的子元素的下面，这是因为father-two会紧跟father-one的下边界（即红色下边框线）。
这显然不是我们需要的效果，我们希望最终的页面效果应该是这样：
son-one
son-two
son-three
所以现在我们需要一种技术可以让父元素包住浮动的子元素，这种技术被称为清除浮动。
清除浮动
清除浮动的方法很多，这里我们只需要掌握一种最常用的方法即可，如下CSS代码即是清除浮动的CSS代码：
.clearfix::after{
  content: '';
  display: block;
  clear: both;
}
比如说我们要解决之前案例中的浮动问题，只需要在父盒子上添加clearfix类名即可，具体参见下方代码：
<!-- 添加清除浮动类名 -->
<div class="father-one clearfix">
    <div class="son-one">son-one</div>
    <div class="son-two">son-two</div>
    <div class="son-three">son-three</div>
</div>
2.3 CSS伪类--事件伪类
伪类在页面中随处可见，我们以淘宝首页为例，挑出几个伪类的案例来看看：
看完这三个案例，我们大致对伪类有了一点了解，通俗点说，就是鼠标移动上去，字体颜色、背景颜色或者边框中的一种或多种样式发生了改变；那么如何使得这些样式发生了改变呢？下面我们就来一探究竟。
首先我们要学习的是鼠标移动上去的效果--hover。
hover——鼠标移动上去
要让样式发生变化，首先我们会有一个基础样式，以“优课达”首页为例：

当鼠标移动上去以后，对应的地方，样式会发生改变，最终变成这样：

观察之后，我们发现，每一个小块的背景颜色从白色-->蓝色，文字从黑色-->白色，所以我们要做的就是在鼠标箭头移动上去以后，完成这两种状态的转换，能完成这种转换过程的就是伪类，具体代码如下：
li:hover{
    background-color: #47A0FC;
    color: white;
}
经过上述步骤之后，我们就会完成如下效果：

最后我们通过代码演示来看一下最终的效果：
active——鼠标点击时
active：鼠标点击时候的效果，这个效果在超链接中比较常见，注意这里的点击是点住鼠标不松开。
在hover的基础上，我们来再添加一个active伪类，实现下图所示效果：

首先需要用选择器选中要添加伪类的标签，ul>li.
然后在选择器后面添加对应的伪类，这里我们要添加的是active
ul>li:active{
    /* 要改变的效果 */
}
最后在花括号内添加要改变的样式:
ul>li:active{
    /* 要改变的效果 */
    color: black;
}
下面我们通过代码演示来看一下最终的效果：
注意：
hover一定要在active之前，否则不会生效。
/* 正确 */
a:hover{}
a:active{}
/* 错误 */
a:active{}
a:hover{}
focus——获取焦点后
focus:获取焦点的伪类，一般用于具有焦点的元素，比如input，比如我们可以让input获取到焦点以后，改变input的边框颜色。

实现步骤在这里就不详细描述，我们可以通过代码演示来看一下最终的效果：


<!--
**hh** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
