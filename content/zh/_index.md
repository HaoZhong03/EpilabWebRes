---
# 首页配置
# 留空 title 将默认使用 config/_default/hugo.yaml 中定义的站点标题 (Epilab)
title: 首页
date: 2026-03-05
type: landing # 本页布局：落地页

sections:

# 使用 slider（幻灯片/轮播图）区块
  - block: slider
    content: # 幻灯片内容列表
      slides:
      # 大图片
      - title: 
        content: 
        align: center # 文字对齐方式：居中
        background:
          image:
            filename: header_2025.jpg
            filters:
              brightness: 1
          position: right # 图片对齐位置
          color: '#666' # 兜底背景颜色

      # 幻灯片一
      - title: 👋 Welcome to the group
        content: Take a look at what we're working on...
        align: center # 文字对齐方式：居中
        background:
          image:
            filename: cow.png
            filters:
              brightness: 0.7
          position: right # 图片对齐位置
          color: '#666' # 兜底背景颜色

      # 幻灯片二
      - title: Lunch & Learn ☕️
        content: 'Share your knowledge with the group and explore exciting new topics together!'
        align: left
        background:
          image:
            filename: contact.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'

    design: # 设计参数
      slide_height: 'calc(100vw / 2.22)' # 幻灯片高度，按视口宽度的 50%：保持(20:19) 比例
      is_fullscreen: false # 全屏模式
      loop: true # 是否自动循环播放
      interval: 5000 # 幻灯片切换的时间间隔（单位：毫秒）

# 区块一：顶部区域，用于展示欢迎语和大图
  - block: markdown 
    content:
      title: 
      text: |
        # **欢迎来到 EpiLab**
        这是一段占位文字，介绍 EpiLab 的历史、使命和研究方向。可以在这里添加更多关于实验室的信息，吸引访问者继续浏览网站。

        👇向下探索更多👇

# 汇总列表（news）
  - block: collection 
    content:
      title: 最新资讯
      subtitle: 查看我们的新闻和最新动态。
      text:
      count: 5 # 数量限制
      filters: # 过滤选项
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc # 按时间倒序排列
      page_type: news # 指定汇总 content/news/ 下的内容
    design:
      view: card # 卡片式显示
      columns: '1' # 设置为单列布局


# 汇总列表（publication）
  - block: collection 
    content:
      title: 最新成果
      subtitle: 探索我们的最新开创性工作。
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article' # 仅过滤出类型为 'article' 的内容
    design:
      view: citation # 使用标准的学术引用样式显示
      columns: '1'

# 底部按钮
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
