---
# 活动或活动的标题
title: '[template]Example Event'
draft: true # 是否为草稿，若是则不渲染
# 活动所属的会议、讲座或组织名称
event: Wowchemy Conference
# 活动相关的官方网址
event_url: https://example.org
# 活动举办的具体地点名称
location: Wowchemy HQ
# 详细地址信息
address:
  street: 450 Serra Mall
  city: Stanford
  region: CA
  postcode: '94305'
  country: United States

# 活动的简短摘要（显示在列表页面）
summary: An example event.
# 活动的详细摘要或简介
abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# 活动开始和结束时间
# 结束时间可以通过注释隐藏
date: '2030-06-01T13:00:00Z'
date_end: '2030-06-01T15:00:00Z'
# 是否为全天活动
all_day: false

# 页面发布日期（非活动举办日期）
publishDate: '2017-01-01T00:00:00Z'

# 活动的演讲者或负责人
# 若已创建作者个人资料，填入其文件夹名（如 admin）即可链接
authors: [admin]
# 活动标签，用于分类和搜索
tags: []

# 是否设为精选活动？（设置为 true 会在首页精选组件中突出显示）
featured: false

# 活动配图设置
image:
  # 图片说明及版权信息
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  focal_point: Right

# 相关资源链接（留空则不显示对应按钮）
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Markdown 幻灯片（可选）
# 填入 content/slides/ 目录下对应的文件名（不含扩展名）
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# 关联项目（可选）
# 填入项目文件夹名，可将此活动与特定科研项目关联
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Slides can be added in a few ways:

- **Create** slides using Wowchemy's [_Slides_](https://docs.hugoblox.com/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://docs.hugoblox.com/writing-markdown-latex/).

Further event details, including page elements such as image galleries, can be added to the body of this page.
