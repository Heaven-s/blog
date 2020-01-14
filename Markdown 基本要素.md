# Markdown 基本要素

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

```markdown
# 这个标题拥有 1 个 id {#my_id}

# 这个标题有 2 个 classes {.class1 .class2}
```
