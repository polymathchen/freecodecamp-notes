HTML——代表超文本标记语言，是一种用于创建网页的标记语言。当你访问一个网站并看到段落、标题、链接、图像和视频等内容时，那就是 HTML。

开始标签和结束标签都以左尖括号（`<`）开头，以右尖括号（`>`）结尾，标签名称位于这两个尖括号之间
结束标签的左尖括号后紧跟着一个正斜杠（`/`）。 有些 HTML 元素没有结束标签。 这些被称为空元素。
没有闭合标签的元素称为 空元素


```HTML
<h1> main heading element </h1>

<img> # 空元素

```


注释能让你在不影响浏览器显示的情况下留下信息。 它也能让你的代码失效。 A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.

这是一个包含文本 `TODO: Remove h1` 的评论示例：

示例代码

```html
<!-- TODO: Remove h1 -->
```

关注点分离是一种设计原则，将程序分成不同的部分，每个部分处理一个单独的关注点。
## 影响SEO

SEO，即搜索引擎优化，是一种优化网页使其在搜索引擎中更易被发现并排名更高的做法。提升网站 SEO 的一种方法是使用 `meta` 元素为网页提供简短的描述。将 `name` 属性设置为 `description` 可确保浏览器、搜索引擎和其他网页工具正确解释这些元数据。`content` 属性是你放置描述的地方
###  开放图谱标签的作用


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

### 元素
- `head` 元素用于包含关于文档的元数据，如它的标题、样式表链接和脚本。 元数据是不直接显示在页面上的关于页面的信息。
- `title` 元素决定浏览器在页面的标题栏或选项卡中显示的内容
- `section` 元素用于在文档中定义各部分，如章节、页眉、页脚或文档的任何其他部分。 它是一个对 SEO 和无障碍有帮助的语义化元素。
-  `ul` 元素  创建一个无序项目列表
-   `a` 元素，也称为锚点元素，用于创建超链接。`a` 标签的开始和结束标签之间的文本是用户点击以导航的可点击部分
- `li` 元素用于在有序或无序列表中创建列表项。
- `figure` 元素代表自包含的内容，允许将图像与标题相关联。
- 图题（`figcaption`）元素用于添加标题来描述 `figure` 元素中包含的图像。
-  `em` 元素——强调一个特定的单词或短语
- 有序列表（`ol`）的代码类似于无序列表，但有序列表中的列表项在显示时是编号的
- `strong` 元素用于表示某些文本非常重要或紧急。
- `footer` 元素用于定义文档或章节的页脚。 页脚通常包含文档作者信息、版权数据、使用条款链接、联系信息等
- `div` 元素用作容器以分组其他元素  `section` 元素比没有语义的 `div` 元素具有语义意义
- `id` 属性为 HTML 元素添加唯一标识符。 `id` 属性值应仅包含字母、数字、下划线和破折号。与 `id` 属性不同，`class` 属性值不需要唯一，可以包含空格。
- `script` 元素用于嵌入可执行代码。 大多数开发人员将使用它来执行 JavaScript 代码。 JavaScript 是用来为你的网页添加交互性的。 使用 JavaScript 的常见示例包括交互式游戏、图像滑块和实时验证用户输入的动态表单。



## 公式化

### Link 元素在HTML中的作用
`link` 元素用于链接样式表和网站图标等外部资源。 以下是为外部 CSS 文件使用 `link` 元素的基本语法：

```html
<link rel="stylesheet" href="./styles.css" />
```

`rel` 属性用于指定链接资源与 HTML 文档之间的关系。 在这种情况下，我们需要指定该链接资源为 `stylesheet`。

将 HTML 和 CSS 分置于不同的文件中被视为最佳实践。 开发人员将使用 `link` 元素来链接外部 CSS 文件，而不是在 HTML 文档中编写所有内容。

`href` 属性用于指定外部资源 URL 的位置。

示例中的 `.` 后跟一个斜线告诉计算机在当前文件夹或目录中查找 `styles.css` 文件。

`link` 元素应放在 `head` 元素内，如下例所示：

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Examples of the link element</title>
  <link rel="stylesheet" href="./styles.css" />
</head>
```

在专业代码库中，你经常会看到多个 `link` 元素，它们链接到不同的样式表、字体和图标。下面是一个使用 `link` 元素链接到名为 _Playwrite Cuba_ 的外部 Google 字体的示例：

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Playwrite+CU:wght@100..400&display=swap"
  rel="stylesheet"
/>
```

Google 字体是一套免费的开源自定义字体，你可以在任何项目中使用。 你可以选择要使用的字体，Google 会为你提供必要的 HTML 和 CSS 代码。 在这个示例中，`rel` 属性的 `preconnect` 值告诉浏览器，要与 `href` 属性中指定的值提前建立连接。 这样做是为了加快这些外部资源的加载时间。

`link` 元素的另一个常见用例是链接到图标。 下面是一个链接到 favicon 的示例：

```html
<link rel="icon" href="favicon.ico" />
```

favicon 是 favorite icon（收藏夹图标）的缩写，通常是在浏览器标签（页）中显示在网站标题旁边的小图标。许多网站会使用 favicon 来显示他们的品牌图标。

### HTML模板
 HTML 模板——就像一个现成的网页模板。 Think of it as the foundation of a house. 模板包括每个 HTML 文档所需的基本结构和重要元素。 节省时间，并有助于确保页面设置正确。 这是一个示例：

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta
       name="viewport"
       content="width=device-width, initial-scale=1.0" />
    <title>freeCodeCamp</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  <body>
  </body>
</html>
```

模板的关键部分。 首先，是 `DOCTYPE` 声明：

```html
<!DOCTYPE html>
```

它会告诉浏览器你使用的 HTML 版本。 接下来，是 `html` 标签：

```html
<!DOCTYPE html>
<html lang="en">
  <!--All other elements go inside here-->
</html>
```

它包裹着你所有的内容，并且可以指定页面的语言。在 `html` 标签内，你会发现两个主要部分，`head` 和 `body`：

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <!--Important metadata goes here-->
  </head>
  <body>
    <!--Headings, paragraphs, images, etc. go inside here-->
  </body>
</html>
```

`head` 部分包含重要的幕后信息：

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document Title Goes Here</title>
  <link rel="stylesheet" href="./styles.css" />
</head>
```

你网站的元数据，包含在 `meta` 元素中，其中包含字符编码等详细信息，以及 Twitter 等网站应如何预览你的页面链接。 你网站的标题，可在 `title` 元素中找到，它决定了显示在浏览器标签页或窗口中的文本。 最后，你通常会在 `head` 部分使用 `link` 元素链接页面的外部样式表。

`body` 部分——放置所有内容的地方：

```html
<body>
  <h1>I am a main title</h1>
  <p>Example paragraph text</p>
</body>
```


### UTF-8 字符编码
UTF-8 —— UCS 转换格式 8，是一种在网络上广泛使用的标准化字符编码。字符编码是计算机用来将字符作为数据保存的方法。本质上，网页上的所有文本都是作为一个或多个字节保存的字符序列。在计算机中，字节是由 8 位（二进制位）组成的数据单位。UTF-8 支持 Unicode 字符集中的每个字符，这包括所有书写系统、语言和技术符号中的字符和符号。下面是使用带有 `charset` 属性的 `meta` 元素将字符编码设置为 `UTF-8` 的示例：

```html
<meta charset="UTF-8" />
```

通过将字符编码设置为 UTF-8，可确保页面上正确显示重音 `"e"` 字符（`é`）。 下面是使用 UTF-8 字符编码的扩展代码示例：

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Examples of the UTF-8 encoding</title>
  </head>
  <body>
    <p>Café</p>
  </body>
</html>
```