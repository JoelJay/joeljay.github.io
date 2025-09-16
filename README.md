# 我的GitHub Pages

这是我的个人GitHub Pages网站，用于展示我的项目、博客和技术分享。

## 🚀 功能特性

- 📱 响应式设计，支持移动端和桌面端
- 🎨 现代化的UI设计
- ⚡ 快速加载和优化的性能
- 🔍 SEO友好的结构
- 📝 博客文章展示
- 💼 项目作品集
- 📧 联系方式

## 🛠️ 技术栈

- **HTML5** - 语义化标记
- **CSS3** - 现代样式和动画
- **JavaScript (ES6+)** - 交互功能
- **Font Awesome** - 图标库
- **GitHub Pages** - 静态网站托管

## 📁 项目结构

```
github-pages/
├── index.html              # 主页面
├── assets/                 # 静态资源
│   ├── css/
│   │   └── style.css      # 主样式文件
│   ├── js/
│   │   └── main.js        # 主JavaScript文件
│   └── images/            # 图片资源
│       ├── hero-image.jpg
│       ├── post-1.jpg
│       ├── post-2.jpg
│       └── favicon.ico
├── blog/                  # 博客文章
├── projects/              # 项目展示
├── about/                 # 关于页面
├── contact/               # 联系页面
├── .well-known/           # 网站验证文件
│   └── assetlinks.json
├── .gitignore            # Git忽略文件
└── README.md             # 项目说明
```

## 🚀 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/你的用户名/你的用户名.github.io.git
cd 你的用户名.github.io
```

### 2. 自定义内容

1. **修改个人信息**
   - 编辑 `index.html` 中的标题、描述和作者信息
   - 更新社交媒体链接
   - 替换占位符图片

2. **添加博客文章**
   - 在 `blog/` 目录下创建新的HTML文件
   - 更新主页面的最新文章部分

3. **添加项目展示**
   - 在 `projects/` 目录下创建项目页面
   - 更新主页面的项目链接

### 3. 部署到GitHub Pages

1. 将代码推送到GitHub仓库
2. 在仓库设置中启用GitHub Pages
3. 选择主分支作为发布源
4. 访问 `https://你的用户名.github.io` 查看网站

## 🎨 自定义样式

### 颜色主题

在 `assets/css/style.css` 中修改CSS变量来更改主题颜色：

```css
:root {
    --primary-color: #3498db;
    --secondary-color: #2c3e50;
    --accent-color: #e74c3c;
    --text-color: #333;
    --bg-color: #fff;
}
```

### 字体

可以通过修改CSS中的 `font-family` 属性来更改字体：

```css
body {
    font-family: 'Your Font', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
```

## 📝 添加新内容

### 添加博客文章

1. 在 `blog/` 目录下创建新的HTML文件
2. 使用以下模板结构：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>文章标题 - 我的GitHub Pages</title>
    <link rel="stylesheet" href="/assets/css/style.css">
</head>
<body>
    <!-- 导航栏 -->
    <nav class="navbar">
        <!-- 导航内容 -->
    </nav>
    
    <!-- 文章内容 -->
    <main class="container">
        <article class="blog-post">
            <header>
                <h1>文章标题</h1>
                <div class="post-meta">
                    <span class="post-date">发布日期</span>
                    <span class="post-category">分类</span>
                </div>
            </header>
            <div class="post-content">
                <!-- 文章内容 -->
            </div>
        </article>
    </main>
    
    <!-- 页脚 -->
    <footer class="footer">
        <!-- 页脚内容 -->
    </footer>
</body>
</html>
```

### 添加项目展示

1. 在 `projects/` 目录下创建项目页面
2. 更新主页面的项目链接和展示内容

## 🔧 开发工具

### 本地开发

可以使用任何静态文件服务器来本地预览网站：

```bash
# 使用Python
python -m http.server 8000

# 使用Node.js
npx serve .

# 使用Live Server (VS Code扩展)
# 右键点击index.html选择"Open with Live Server"
```

### 代码格式化

建议使用以下工具来保持代码格式一致：

- **Prettier** - 代码格式化
- **ESLint** - JavaScript代码检查
- **Stylelint** - CSS代码检查

## 📱 响应式设计

网站已经针对以下设备进行了优化：

- 📱 手机 (320px - 768px)
- 📱 平板 (768px - 1024px)
- 💻 桌面 (1024px+)

## 🔍 SEO优化

网站已经包含了基本的SEO优化：

- 语义化HTML结构
- Meta标签优化
- Open Graph标签
- Twitter Card标签
- 结构化数据（可扩展）

## 🚀 性能优化

- 图片懒加载
- CSS和JavaScript压缩
- 字体优化
- 缓存策略

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 📞 联系方式

- GitHub: [@你的用户名](https://github.com/你的用户名)
- Twitter: [@你的用户名](https://twitter.com/你的用户名)
- LinkedIn: [你的用户名](https://linkedin.com/in/你的用户名)
- Email: your.email@example.com

---

⭐ 如果这个项目对你有帮助，请给它一个星标！
