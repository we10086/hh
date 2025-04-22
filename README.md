## Hi there 👋
开始
基础
<MARKDOWN>
# HTML & CSS 基础教程
## 一、HTML基础结构
### 1. 文档类型声明
```html
<!DOCTYPE html>
作用：声明文档类型，指示浏览器使用HTML5解析页面
特性：
必须是文档第一行
对大小写不敏感
没有闭合标签
2. HTML根元素
<HTML>
<html lang="en">...</html>
作用：定义HTML文档根元素
特性：
lang属性定义文档语言（例：en表示英文）
包含<head>和<body>两大部分
3. 标签属性规则
格式：key="value"
多个属性用空格分隔
常见属性：
<HTML>
<div class="container" id="main" style="color:red"></div>
二、文档结构
1. 头部 <head>
<HTML>
<head>
  <title>页面标题</title>
  <!-- 元信息/样式表等 -->
</head>
必须包含且只能有一个<title>
常用元数据：字符编码声明
<HTML>
<meta charset="UTF-8">
2. 主体 <body>
<HTML>
<body>
  <!-- 页面展示内容 -->
</body>
3. HTML注释
<HTML>
<!-- 注释内容 -->
不显示在浏览器中
三、常用标签使用
1. 图片 <img>
<HTML>
<img src="image.jpg" alt="图片描述">
关键属性：
src: 图片路径
alt: 替代文本
title: 悬浮提示
2. 超链接 <a>
<HTML>
<a href="https://example.com" target="_blank" title="示例链接">
  点击跳转
</a>
属性：
href: 目标URL
target:
_self（默认，当前页）
_blank（新标签页）
3. 列表
有序列表：

<HTML>
<ol>
  <li>第一项</li>
  <li>第二项</li>
</ol>
无序列表：

<HTML>
<ul>
  <li>项目1</li>
  <li>项目2</li>
</ul>
四、表单元素
1. 表单容器
<HTML>
<form action="/submit" method="POST">
  <!-- 表单控件 -->
</form>
2. 输入框
<HTML>
<input type="text" 
       placeholder="输入提示"
       name="username"
       value="默认值"
       readonly>
3. 选择菜单
<HTML>
<select name="city">
  <option value="bj">北京</option>
  <option value="sh" selected>上海</option>
</select>
4. 复选框/单选框
<HTML>
<input type="checkbox" name="interest" value="coding"> 编程
<input type="radio" name="gender" value="male"> 男
5. 按钮
<HTML>
<button type="submit">提交</button>
五、CSS样式基础
1. 行内样式
<HTML>
<p style="font-size: 16px; color: #333;">示例文本</p>
2. 文字样式
<CSS>
/* 文字大小 */
font-size: 14px;
/* 字体粗细 */
font-weight: bold;
/* 文字颜色 */
color: #ff0000;
/* 对齐方式 */
text-align: center;
/* 行高 */
line-height: 1.5;
/* 字间距 */
letter-spacing: 2px;
/* 字体 */
font-family: Arial, sans-serif;
3. 伪类示例
<CSS>
/* 链接悬浮效果 */
a:hover {
  color: red;
}
/* 输入框聚焦效果 */
input:focus {
  border-color: blue;
}
/* 清除浮动 */
.clearfix::after {
  content: '';
  display: block;
  clear: both;
}
六、HTML5 语义化标签
<HTML>
<header>页眉</header>
<nav>导航栏</nav>
<main>
  <section>内容区块</section>
</main>
<aside>侧边栏</aside>
<footer>页脚</footer>
七、高级技巧
1. 伪元素应用
<CSS>
.icon::before {
  content: '';
  display: inline-block;
  width: 24px;
  height: 24px;
  background: url(icon.png);
}
.list-item::after {
  content: "→";
  margin-left: 8px;
}
2. 定位示例
<CSS>
.position-demo {
  position: relative;
}
.position-demo::before {
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
}

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
