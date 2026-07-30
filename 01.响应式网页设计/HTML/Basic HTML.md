HTML——代表超文本标记语言，是一种用于创建网页的标记语言。当你访问一个网站并看到段落、标题、链接、图像和视频等内容时，那就是 HTML。

开始标签和结束标签都以左尖括号（`<`）开头，以右尖括号（`>`）结尾，标签名称位于这两个尖括号之间
结束标签的左尖括号后紧跟着一个正斜杠（`/`）。 有些 HTML 元素没有结束标签。 这些被称为空元素。

```HTML
<h1> main heading element </h1>
```



## 属性

属性是用于调整 HTML 元素行为的特殊值。

属性是放置在 HTML 元素开始标签内的一个值。 属性提供元素的附加信息，或指定元素的行为方式。 以下是属性的基本语法：

```html
<element attribute="value"></element>
```

属性名称后跟一个等号（`=`）和一个带引号的值。 值可以是字符串或数字，具体取决于属性。

第一个示例使用了 `href` 和 `target` 属性。`href` 属性指定链接的 URL，`target` 属性指定打开链接的位置。

**注意：** `a` 元素，也称为锚点元素，用于创建超链接。`a` 标签的开始和结束标签之间的文本是用户点击以导航的可点击部分。

启用交互式编辑器并将 `href="https://www.freecodecamp.org/news/"` 更改为 `href="https://www.freecodecamp.org"`。现在，当你点击交互式编辑器中的链接时，你将在新的浏览器标签（页）中看到 freeCodeCamp 主页。

```html
<a href="https://www.freecodecamp.org/news/" target="_blank">Visit freeCodeCamp</a>
```

如果没有 `href` 属性，链接将无法工作，因为没有目标 URL。所以你必须包含这个 `href` 属性以使链接生效。`target="_blank"` 启用链接在新的浏览器标签（页）中打开。你将在后续课程中学习更多关于 `target` 属性的内容。

其他常见的属性有 `src` 和 `alt`，或称备选属性，分别用于指定图像的来源和为图像提供备选描述性文本。

在 HTML 中常见的布尔属性，例如 `disabled`、`readonly` 和 `required`。 这些属性用于指定元素的状态，如禁用、只读或必填