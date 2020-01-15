# Markdown 基本要素

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=true} -->

<!-- code_chunk_output -->

1. [Markdown 基本要素](#markdown-基本要素)
    1. [什么是 Markdown](#什么是-markdown)
    2. [语法说明](#语法说明)
        1. [标题](#标题)
        2. [强调](#强调)
        3. [列表](#列表)
        4. [添加图片](#添加图片)
        5. [链接](#链接)
        6. [引用](#引用)
        7. [分割线](#分割线)
        8. [行内代码](#行内代码)
        9. [代码块](#代码块)
        10. [语法高亮](#语法高亮)
            1. [代码行数](#代码行数)
            2. [高亮代码行数](#高亮代码行数)
        11. [任务列表](#任务列表)
        12. [表格](#表格)
        13. [Emoji & Font-Awesome](#emoji-font-awesome)
        14. [上标](#上标)
        15. [下标](#下标)
        16. [脚注](#脚注)
        17. [缩略](#缩略)
        18. [标记](#标记)
        19. [数学](#数学)

<!-- /code_chunk_output -->

推荐安装 VS Code `markdown-preview-enhanced` 预览插件、`markdownlint` 格式检查插件 [参考地址](https://shd101wyy.github.io/markdown-preview-enhanced)

## 什么是 Markdown

`Markdown` 是一种文本格式。你可以用它来控制文档的显示。使用 markdown，你可以创建粗体的文字，斜体的文字，添加图片，并且创建列表 等等。基本上来讲，Markdown 就是普通的文字加上 `#` 或者 `*` 等符号。

## 语法说明

### 标题

```markdown
  # 这是 <h1> 一级标题

  # 这是 <h2> 二级标题

  # 这是 <h3> 三级标题

  # 这是 <h4> 四级标题

  # 这是 <h5> 五级标题

  # 这是 <h6> 六级标题
```

如果你想要给你的标题添加 `id` 或者 `class`，请在标题最后添加 `{#id .class1 .class2}`。例如：

> _这是一个 **MPE** 扩展的特性。_

```markdown
  # 这个标题拥有 1 个 id {#my_id}

  # 这个标题有 2 个 classes {.class1 .class2}
```

### 强调

```markdown
  *这会是 斜体 的文字*
  _这会是 斜体 的文字_

  **这会是 粗体 的文字**
  __这会是 粗体 的文字__

  _你也 **组合** 这些符号_

  ~~这个文字将会被横线删除~~
```

### 列表

- 无序列表
  
```markdown
  - Item 1
  - Item 2
    - Item 2a
    - Item 2b
```

- 有序列表
  
```markdown
  1. Item 1
  1. Item 2
  1. Item 3
    1. Item 3a
    1. Item 3b
```

### 添加图片

<img src="https://cn.vuejs.org/images/logo.png" width="50" height="50" />

```markdown
  ![GitHub Logo](https://cn.vuejs.org/images/logo.png)
  Format: ![Alt Text](url)
```

### 链接

[GitHub](https://github.com)

```markdown
  http://github.com - 自动生成！
  [GitHub](http://github.com)
```

### 引用

> Vue是一套用于构建用户界面的渐进式框架

```markdown
  正如 Kanye West 所说：

  > We're living the future so
  > the present is our past.
```

### 分割线

---

```markdown
  如下，三个或者更多的

  ---

  连字符

  ---

  星号

  ---

  下划线
```

### 行内代码

```markdown
  我觉得你应该在这里使用
  `<addr>` 才对。
```

### 代码块

你可以在你的代码上面和下面添加 ` ``` ` 来表示代码块

### 语法高亮

你可以给你的代码块添加任何一种语言的语法高亮

例如，给 ruby 代码添加语法高亮：

\`\`\`ruby<br/>
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html<br/>
\`\`\`

会得到下面的效果：

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

#### 代码行数

如果你想要你的代码块显示代码行数，只要添加 line-numbers class 就可以了。

例如：

```javascript {.line-numbers}
function add(x, y) {
  return x + y
}
```

#### 高亮代码行数

你可以通过添加 highlight 属性的方式来高亮代码行数：

```javascript {.line-numbers highlight=2}
function add(x, y) {
  return x + y
}
```

### 任务列表

```markdown
- [ ] @mentions, #refs, [links](https://github.com), **formatting**, and ~~tags~~ supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```

- [ ] @mentions, #refs, [links](https://github.com), **formatting**, and ~~tags~~ supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

### 表格

```markdown
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

### Emoji & Font-Awesome

> 只适用于 markdown-it parser 而不适用于 pandoc parser。 缺省下是启用的。你可以在插件设置里禁用此功能。

:smile:
:fa-car:

```markdown
:smile:
:fa-car:
```

### 上标

30^th^

```markdown
30^th^
```

### 下标

H~2~O

```markdown
H~2~O
```

### 脚注

Content [^1]

[^1]: Hi! This is a footnote

```markdown
Content [^1]

[^1]: Hi! This is a footnote
```

### 缩略

Content [^1]

_[HTML]: Hyper Text Markup Language
_[W3C]: World Wide Web Consortium
The HTML specification
is maintained by the W3C.

```markdown
_[HTML]: Hyper Text Markup Language
_[W3C]: World Wide Web Consortium
The HTML specification
is maintained by the W3C.
```

### 标记

==marked==

```markdown
==marked==
```

### 数学

**Markdown Preview Enhanced** 使用 [KaTeX](https://github.com/Khan/KaTeX) 或者 [MathJax](https://github.com/mathjax/MathJax) 来渲染数学表达式。

KaTeX 拥有比 MathJax 更快的性能，但是它却少了很多 MathJax 拥有的特性。你可以查看 [KaTeX supported functions/symbols](https://khan.github.io/KaTeX/function-support.html) 来了解 KaTeX 支持那些符号和函数。

默认下的分隔符：

- `$...$` 或者 `\(...\)` 中的数学表达式将会在行内显示。
- `$$...$$` 或者 `\[...\]` 或者 <code>```math</code> 中的数学表达式将会在块内显示。

![](https://cloud.githubusercontent.com/assets/1908863/14398210/0e408954-fda8-11e5-9eb4-562d7c0ca431.gif)

你可以在 **插件设置中** 选择数学渲染引擎以及分隔符。

你也可以通过 <kbd>cmd-shift-p</kbd> 然后选择 `Markdown Preview Enhanced: Open Mathjax config` 命令来打开 Mathjax 配置文件。
