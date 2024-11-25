# 基于 VitePress 的个人博客

这是一个使用 VitePress 构建的个人博客项目，包含了文章管理、评论系统、友链、搜索等功能。

## 特性

- 📝 基于 VitePress 构建
- 💬 集成 Giscus 评论系统
- 🔍 本地搜索功能
- 🖼️ 图片预览功能
- 🌙 深色模式支持
- 🔗 友链系统
- 💫 一言 API 集成
- 📱 响应式设计

## 项目结构

```
blog
├── .vitepress
│ ├── config.mjs # 主配置文件
│ ├── config
│ │ ├── nav.js # 导航配置
│ │ ├── sidebar.js # 侧边栏配置
│ │ ├── search.js # 搜索配置
│ │ └── meta.js # 元信息配置
│ └── theme
│ ├── style.css # 主题样式
│ ├── components # 自定义组件
│ └── data # 数据文件
├── src
│ ├── about # 关于页面
│ ├── blog # 博客文章
│ ├── friends # 友链页面
│ └── todo # TODO 页面
└── public # 静态资源
```

## 开发环境要求

- Node.js >= 16
- pnpm >= 8

## 使用说明

1.克隆仓库

```bash
git clone https://github.com/yourusername/blog.git
cd blog
```

2.安装依赖

```bash
pnpm install
```

3.本地开发

```bash
pnpm docs:dev
```

4.构建

```bash
pnpm docs:build
```

5.部署
构建后的文件在 dist 目录
可以配置 Nginx 将网站根目录指向 dist 文件夹
具体配置可参考 [Nginx 配置](https://blog.honahec.cc/blog/nginx.html)

## 主要功能

1. 文章系统

- 支持 Markdown 写作
- 自动生成目录
- 代码高亮
- 图片预览

2. 评论系统

- 基于 Giscus 的评论功能
- GitHub Discussions 数据同步

3. 友链系统

- 友链展示
- 友链申请

4. 其他功能

- 本地搜索
- 一言 API 集成
- 深色模式切换
- 响应式设计

## 自定义配置

1. 导航栏配置
   编辑 `.vitepress/config/nav.js`
2. 侧边栏配置
   编辑 `.vitepress/config/sidebar.js`
3. 搜索配置
   编辑 `.vitepress/config/search.js`
4. 主题配置
   编辑 `.vitepress/theme/style.css`

## 贡献

欢迎提交 Issue 和 Pull Request
