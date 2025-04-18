# 个人技术博客

这是一个基于Astro构建的个人技术博客，主要分享技术学习和ACGN相关的技术文章、教程和经验分享。

## 🔧 技术栈

- 构建框架: [Astro](https://astro.build)
- 主题: 基于[Fuwari](https://github.com/saicaca/fuwari)定制

## 🚀 本地运行

1. 克隆此仓库

   ```bash
   git clone <your-repo-url>
   cd AstroBlog
   ```

2. 安装依赖

   ```bash
   pnpm install
   pnpm add sharp
   ```

3. 启动开发服务器

   ```bash
   pnpm dev
   ```

4. 创建新文章

   ```bash
   pnpm new-post <文章文件名>
   ```

   然后在 posts 目录下编辑新创建的文章

## 📝 文章格式

文章使用Markdown格式，需要在文件开头添加frontmatter信息：

```yaml
---
title: 文章标题
published: 2025-04-10
description: 文章描述，会显示在首页的文章卡片上
image: ./assets/cover.jpg
tags: [标签1, 标签2]
category: 分类名称
draft: false
---
```

## 📦 构建与部署

构建静态网站：

```bash
pnpm build
```

预览构建结果：

```bash
pnpm preview
```

## 📋 可用命令

| 命令                  | 说明                            |
|:---------------------|:--------------------------------|
| `pnpm dev`           | 启动开发服务器，地址为`localhost:4321` |
| `pnpm build`         | 构建生产站点到`./dist/`目录        |
| `pnpm preview`       | 在部署前本地预览构建结果            |
| `pnpm new-post <文件名>` | 创建新文章                       |
