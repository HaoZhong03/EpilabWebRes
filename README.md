# EPILAB门户网页项目

本项目为[中国农业大学](https://www.cau.edu.cn/)[动物科学技术学院](https://cast1.cau.edu.cn/)动物遗传育种系EPILAB团队的学术网页资源仓库，由团队中Zhong、Chen、Jiang三人进行维护。拟使用的域名为：cau666.yyEpiLab.cn。

项目基于模板[Hugo Research Group Theme](https://github.com/wowchemy/starter-hugo-research-group)进行构建。

## 项目文件树结构
```
.
├── .github # GitHub 平台相关
├── assets 资源与样式
├── config # 站点配置
├── content # 网站的所有展示内容
│   ├── _index.md # 首页
│   ├── admin 
│   ├── authors # 成员介绍，每人一个文件夹
│   ├── contact # 联系方式
│   ├── event # 活动
│   ├── people # 成员列表
│   ├── post # 动态
│   ├── publication # 学术成果
│   └── tour # 项目展示
├── images # 其他图片资源
├── static # 其他静态资源
├── .gitignore
├── .editorconfig
├── go.mod
├── go.sum
├── LICENSE.md
├── netlify.toml
├── preview.png
├── README.md
└── theme.toml
```
## 本项目用到的工具或软件

维护该项目主要涉及内容编辑、本地预览和自动化部署三个方面。根据项目文件中的配置和脚本，你需要准备以下工具和软件：

1. 本地开发：

- Hugo (Extended版)：用于在本地预览和构建静态文件。
- Go：Hugo的依赖。

- Git & GitHub：代码托管中心。

- Python 3.12+ & Academic CLI：用于运行 academic 脚本，将 publications.bib 自动转换为网站的论文页面。

2. 服务器部署：

- Web 服务器 (Nginx 或 Apache)：在 ECS 上部署，用于托管 Hugo 生成的 public/ 静态文件夹。

- 终端工具 (如 Termius, PuTTY, iTerm2)：通过 SSH 登录服务器进行配置。

- 传输工具 (如 FileZilla, WinSCP)：用于将本地生成的 public/ 文件夹手动上传到服务器。

- GitHub Actions (SSH 插件)：在代码推送时自动通过 SSH 将编译后的文件拉取或推送到阿里/腾讯云服务器。

## 项目进行计划：

**3月2日-3月8日**：完善网页整体框架及网页元素，制作信息收集清单及收集表。

**3月9日-3月15日**：收集信息并整理，准备域名购买、备案及服务器部署工作。

**3月16日-3月22日**：微调网站细节，准备上线。