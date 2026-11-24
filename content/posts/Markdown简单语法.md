---
title: "Markdown简单语法"
date: 2026-11-23T14:22:05+08:00
draft: false
categories: ["学习"]
tags: ["Markdown"]
---

一份够用版**Markdown速查**，适合写 Hugo 博客文章。

### 1. 标题
```markdown
# 一级标题
## 二级标题
### 三级标题
```
> 文章正文里一般从 `##` 开始用，`#` 通常留给文章标题。

### 2. 段落与换行
```markdown
这是第一段。

这是第二段。
```
- **空一行** = 新段落。
- 想在同一段内强制换行，行尾加**两个空格**再回车，或直接空一行。

### 3. 强调
```markdown
**加粗**
*斜体*
***加粗斜体***
~~删除线~~
```

### 4. 列表
无序列表：
```markdown
- 苹果
- 香蕉
  - 子项
```
有序列表：
```markdown
1. 第一步
2. 第二步
```

### 5. 链接与图片
```markdown
[必应](https://www.bing.com)
![图片说明](/images/example.png)
```
Hugo 里图片通常放在 `static/images/`，文章里写 `/images/example.png`。

### 6. 代码
行内代码：
```markdown
使用 `pip install requests` 安装。
```
代码块：
````markdown
```python
print("Hello")
```
````
> 三个反引号后写语言名，Hugo 会做语法高亮。

### 7. 引用
```markdown
> 这是一段引用。
> 可以多行。
```

### 8. 分隔线
```markdown
---
```
> 注意：文章开头的 Front Matter 也用 `---`，正文分隔线不要紧贴开头配置区。

### 9. 表格
```markdown
| 名称 | 说明 |
|---|---|
| A | 第一项 |
| B | 第二项 |
```

### 10. 任务列表
```markdown
- [x] 已完成
- [ ] 未完成
```

### 11. 转义特殊符号
想显示 `*`、`#`、`[` 等符号时，前面加反斜杠：
```markdown
\*不是斜体\*
```

### 12. Hugo 文章开头模板
```markdown
---
title: "文章标题"
date: 2026-11-20
draft: false
tags: ["Python", "工具"]
categories: ["技术"]
---

## 小标题

正文内容……
```

### 最常用记住这几条就够了
```markdown
## 标题
**加粗**
- 列表
[链接](https://example.com)
![图片](/images/a.png)
`行内代码`
```python
代码块
```
> 引用
| 表格 | 表格 |
|---|---|
| A | B |
```

写博客时，**空行分段**和**代码块三个反引号**是最容易出错的地方，注意即可。

