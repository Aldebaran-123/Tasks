## 一、HTML 

- **定义与作用**：超文本标记语言，构建网页的 “骨架”，负责页面结构与内容呈现。
- **基础结构**：根标签`<html>`，包含`<head>`（元信息区，如`<title>`页面标题）和`<body>`
- 核心标签
  - 文本类：`<h1>-<h6>`（标题）、`<p>`（段落）、`<strong>`（加粗）、`<em>`（斜体）、`<br>`（换行）、`<hr>`（水平线）。
  - 媒体与链接：`<img>`（图片，含`src`/`alt`/`width`属性）、`<a>`（链接，含`href`/`target`属性）、`<audio>`（音频）。
  - 列表：`<ul>+<li>`（无序列表）、`<ol>+<li>`（有序列表）、嵌套列表。
  - 表格：`<table>`（容器）、`<tr>`（行）、`<td>`（单元格）、`<th>`（表头）、`rowspan`/`colspan`（合并单元格）。
  - 表单：`<form>`（容器）、`<input>`（输入框 / 单选 / 复选 / 按钮）、`<select>+<option>`（下拉菜单）、`<textarea>`（文本域）、`<fieldset>+<legend>`（分组）。
  - 语义化：`<header>`（页头）、`<nav>`（导航）、`<main>`（主体）、`<section>`（区块）、`<article>`（文章）、`<footer>`（页脚）。
- **语法规范**：双标签需闭合，单标签按规范书写，属性名与值需匹配。

------

## 二、CSS 

- **定义与作用**：层叠样式表，负责网页的 “美化”，控制样式、布局与视觉呈现。
- **引入方式**：内联样式（标签`style`属性）、内部样式表（`<head>`中`<style>`标签）、外部样式表（`.css`文件 +`<link>`引入）。
- **选择器**：元素选择器（标签名）、类选择器（`.`+ 类名）、ID 选择器（`#`+ID 名）、通配符选择器（`*`）。
- 核心样式
  - 字体文本：`font-family`（字体）、`font-size`（大小）、`font-weight`（粗细）、`color`（文本颜色）、`text-align`（对齐）、`line-height`（行高）。
  - 背景：`background-color`（纯色）、`background-image`（背景图）、`background-repeat`（重复方式）、`background-size`（尺寸）。
  - 盒子模型：内容区（content）、内边距（padding）、边框（border）、外边距（margin），`margin: 0 auto`实现水平居中。
  - 布局：`float`（浮动，实现横向排列）、`position`（定位：static/relative/absolute/fixed）、`clear`（清除浮动）。
- **语法规范**：选择器 +`{ 属性名: 属性值; }`，分号分隔多个属性，大括号包裹样式代码。

------

## 三、JS 

- **定义与作用**：弱类型脚本语言，负责网页 “交互逻辑”，实现动态效果与数据处理。

- **引入方式**：内联脚本（事件属性，如`onclick`）、内部脚本（`<script>`标签包裹）、外部脚本（`.js`文件 +`<script src>`引入）。

- 基础语法
  - 变量声明：`let`（块级作用域）、`var`（函数级作用域）、`const`（常量）。
  - 数据类型：字符串（string）、数字（number）、布尔值（boolean）、undefined、null。
  - 运算符：算术运算符（`+`/`-`/`*`/`/`/`%`）、赋值运算符（`=`/`+=`）、比较运算符（`==`/`===`/`>`/`<`）、逻辑运算符（`&&`/`||`/`!`）。
  - 流程控制：`if-else`（条件判断）、`switch`（多值匹配）、`for`/`while`/`do-while`（循环）。

- 事件处理
  - 常用事件：`onclick`（点击）、`onmouseover`（鼠标移入）、`oninput`（输入变化）、`onsubmit`（表单提交）。
  - 绑定方式：内联绑定（标签属性）、脚本绑定（通过 DOM 获取元素绑定事件）。


- **输出方式**：`alert()`（弹窗）、`console.log()`（控制台输出）、`document.write()`（页面输出）。
