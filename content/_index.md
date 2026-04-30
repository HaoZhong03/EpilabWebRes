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
      - title: 
        content: 
        align: 
        background:
          image:
            filename: header_2025.jpg
          position: center # 图片对齐位置
          color: '#666' # 兜底背景颜色

      # 幻灯片一
      - title:
        content: 
        align: 
        background:
          image:
            filename: cow.png
          position: center # 图片对齐位置
          color: '#666' # 兜底背景颜色

      # 幻灯片二
      - title: 
        content: 
        align: 
        background:
          image:
            filename: contact.jpg
          position: center
          color: '#666'

    design: # 设计参数
      slide_height: 'calc(100vw / 2.22)' # 幻灯片高度，按视口宽度的 50%：保持(20:19) 比例
      is_fullscreen: false # 全屏模式
      loop: true # 是否自动循环播放
      interval: 5000 # 幻灯片切换的时间间隔（单位：毫秒）

# 区块一：顶部区域，用于展示欢迎语和大图
  - block: markdown 
    content:
      title: 欢迎来到 EpiLab
      text: |
        -	课题组开展奶牛抗乳房炎性状的体内、外模型构建，转录组、表观基因组等功能基因组学数据分析及功能验证等工作，在国内外高水平期刊发表论文150余篇，以第一发明人授权国家发明专利10项，获省部级科研奖励7项。
        - 课题组作为国际 **FarmGTEx**（畜禽基因型-组织表达）研究计划的主要发起人之一，与国内外奶牛遗传育种研究领域的科研人员交流合作密切。前期合作建立了[CattleGTEx数据库](https://cgtex.roslin.ed.ac.uk)，为奶牛复杂性状的遗传机制解析提供了宝贵资源。

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
    # 使用紧凑的列表视图居中显示新闻
      view: 
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
        ### <center>了解关于我们的更多信息
        <br>
        <div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap;">
          <div>{{% cta cta_link="./people/" cta_text="团队介绍" %}}</div>
          <div>{{% cta cta_link="https://github.com/HaoZhong03/EpilabWebRes" cta_text="项目地址" %}}</div>
          <div>{{% cta cta_link="./contact/" cta_text="联系我们" %}}</div>
        </div>
---
