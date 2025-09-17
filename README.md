# Liangjie's Blog

这是我的个人博客网站，基于Jekyll构建，托管在GitHub Pages上。

## 功能特性

- 📝 支持Markdown写作
- 🎨 响应式设计，支持移动端
- 🔍 文章分类和标签
- 📱 现代化UI设计
- ⚡ 快速加载速度
- 🔗 社交媒体链接

## 本地开发

### 环境要求

- Ruby 2.7+
- Bundler

### 安装步骤

1. 克隆仓库
```bash
git clone https://github.com/joeljay/joeljay.github.io.git
cd joeljay.github.io
```

2. 安装依赖
```bash
bundle install
```

3. 启动本地服务器
```bash
bundle exec jekyll serve
```

4. 访问 http://localhost:4000

## 项目结构

```
├── _config.yml          # Jekyll配置文件
├── _layouts/            # 页面布局模板
├── _includes/           # 可重用组件
├── _posts/              # 博客文章
├── about/               # 关于页面
├── blog/                # 博客列表页
├── projects/            # 项目展示页
├── contact/             # 联系页面
├── assets/              # 静态资源
│   ├── css/            # 样式文件
│   ├── js/             # JavaScript文件
│   └── images/         # 图片资源
└── img/                # 文章图片
```

## 写作指南

### 创建新文章

在 `_posts` 目录下创建新的Markdown文件，文件名格式为：`YYYY-MM-DD-文章标题.md`

### 文章头部信息

```yaml
---
title: 文章标题
date: 2024-01-01 12:00:00
categories: [分类1, 分类2]
tags: [标签1, 标签2]
---
```

### 添加图片

将图片放在 `img` 目录下，在文章中使用相对路径引用：

```markdown
![图片描述](/img/图片名称.jpg)
```

## 部署

本网站使用GitHub Pages自动部署，每次推送到main分支都会自动构建和部署。

## 许可证

MIT License

## 联系方式

- 邮箱：huangliangjie110@163.com
- GitHub：[@joeljay](https://github.com/joeljay)