---
# 论文或文章的标题
title: "[template]An example journal article"
draft: true # 是否为草稿，若是则不渲染
authors:
# 作者列表
- admin
- Robert Ford
# 作者备注
author_notes:
- "Equal contribution"
- "Equal contribution"
# 论文发表日期
date: "2015-09-01T00:00:00Z"
doi: ""

# 页面在网站上的发布日期（通常用于排序，非实际发表日期）
publishDate: "2017-01-01T00:00:00Z"

# 出版物类型
# 采用 CSL 标准，常用值包括：article-journal (期刊), paper-conference (会议), book (书籍), report (报告)
publication_types: ["article-journal"]

# 出版物名称
publication: "*Journal of Source Themes, 1*(1)"
publication_short: ""

# 出版物名称
abstract: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam. Quisque risus orci, mollis id ante sit amet, gravida egestas nisl. Sed ac tempus magna. Proin in dui enim. Donec condimentum, sem id dapibus fringilla, tellus enim condimentum arcu, nec volutpat est felis vel metus. Vestibulum sit amet erat at nulla eleifend gravida.

# 简短总结（可选，若填写则显示在列表卡片中，否则默认截取摘要）
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# 标签，用于分类和搜索
tags:
- example
featured: false

# 自定义按钮链接（若下方预设链接不够用，可在此添加）
# links:
# - name: ""
#   url: ""
# 各类资源链接（留空则不显示对应按钮）
url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# 封面图设置
# 需将名为 `featured.jpg/png` 的图片放入该论文文件夹内
image:
  # 图片描述/版权
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  # 图片裁剪焦点
  focal_point: ""
  # 是否仅在预览时显示（不显示在论文详情页顶部）
  preview_only: true

# 关联项目（可选）
# 填入 content/project/ 目录下对应的文件夹名
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# 关联幻灯片（可选）
# 填入 content/slides/ 目录下对应的文件名（不含扩展名）
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

{{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
