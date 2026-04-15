---
title: 团队
date: 2022-10-24

type: landing

sections:
  - block: people
    content:
      title: 成员介绍
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - 教授
          - 副研究员
          - 博士后
          - 博士研究生
          - 硕士研究生
          - 毕业生
      # 按role排序
      sort_by: Params.role
      # 按数字从小到大排序
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: false
---