Google 有一个免费的在线字体库，拥有超过 1600 种字体可供选择。 该网站允许你使用自己的示例文本浏览不同的字体，以帮助你找到合适的字体。 然后，Google Fonts 会为你提供将字体**链接**或**导入**到你的网站所需的**HTML**和**CSS**。

### 查找字体

打开[fonts.google.com](https://fonts.google.com/){:target="_blank"}.

在**Preview**（预览）框中输入一些示例文本

![Google 字体搜索页面。 预览框中有 'Lapis Sarawak' 字样。](images/custom.png)

**注意**示例显示的是你的示例文本。 你可以看到你的文字在所有可用字体下的显示效果。

有许多不同的搜索过滤器可供使用。 你可以按语言或不同的字体属性进行搜索。

向下滚动直到找到你喜欢的字体。 如果你知道要使用的字体的名称，请在主搜索框中输入它。

!['Bangers' 已经输入到了搜索框中。](images/bangers.png)

**注意**你现在可以看到已应用于示例文本的 Bangers 字体的示例。

### 选择你的字体大小

这个示例以 40px 显示

### 获取嵌入代码

点击右上角的 “Get font” （获取字体）按钮。

你将看到你选择的字体。

![选定的字体。](images/selected-font.png)

点击“Get embed code”（获取嵌入代码）按钮。

你可以使用`<link>` 方法或`<import>` 方法。

### 链接方法

![要复制的 HTML。](images/link.png)

将 HTML 代码复制并粘贴到 HTML 文档中的 `<head>` 标签内。

## --- code ---

language: html
filename:
line_numbers:
line_number_start: 1
line_highlights: 2-4
---------------------------------------------------------

  <!-- Import fonts from Google -->

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bangers&display=swap" rel="stylesheet">

\--- /code ---

你需要添加正确的 CSS，以便让 Web 浏览器知道何时使用此字体。

转到您的 `default.css` 文件并找到字体变量（它也可能是包含你选择的调色板的文件，例如 `fiesta.css`）。

添加（或替换）你选择的字体的代码。 在我们的例子中，我们使用 `Bangers, cursive;` 。

## --- code ---

language: css
filename: default.css
line_numbers: true
line_number_start: 15
line_highlights: 16-18
-----------------------------------------------------------

\--body-font: 1.1rem Verdana, sans-serif;
\--header-font: lighter 3rem 'Bangers', cursive;
\--title-font: lighter 2rem 'Bangers', cursive;
\--quote-font: lighter 1.5rem 'Bangers', cursive;

\--- /code ---

### 导入方法

![要复制的 CSS。](images/import.png)

打开 `style.css`。

复制并粘贴顶部的导入代码。

将其添加到 CSS 文件时，请确保在行尾添加分号 `;`。

## --- code ---

language: css
filename: style.css
line_numbers:
line_number_start:
line_highlights:
-----------------------------------------------------

@import url('https://fonts.googleapis.com/css2?family=Bangers&display=swap');

\--- /code ---

打开 `default.css` 并找到字体变量(它也可能是包含你选择的调色板的文件，例如 `fiesta.css`)。

添加（或替换）你选择的字体的代码。 在我们的例子中，我们使用 `Bangers, cursive;` 。

## --- code ---

language: css
filename: default.css
line_numbers: true
line_number_start: 15
line_highlights: 16-18
-----------------------------------------------------------

\--body-font: 1.1rem Verdana, sans-serif;
\--header-font: lighter 3rem 'Bangers', cursive;
\--title-font: lighter 2rem 'Bangers', cursive;
\--quote-font: lighter 1.5rem 'Bangers', cursive;

\--- /code ---