# Personal Tech Blog

This is a personal tech blog built with Astro, mainly sharing technical learning and ACGN-related tech articles, tutorials, and experience.

## 🔧 Tech Stack

- Framework: [Astro](https://astro.build)
- Theme: Customized based on [Fuwari](https://github.com/saicaca/fuwari)

## 🚀 Local Setup

1. Clone this repository

   ```bash
   git clone <your-repo-url>
   cd AstroBlog
   ```

2. Install dependencies

   ```bash
   pnpm install
   pnpm add sharp
   ```

3. Start the development server

   ```bash
   pnpm dev
   ```

4. Create a new post

   ```bash
   pnpm new-post <post-filename>
   ```

   Then edit the newly created post in the `posts` directory.

## 📝 Post Format

Posts use Markdown format. You need to add frontmatter information at the beginning of the file:

```yaml
---
title: Post Title
published: 2025-04-10
description: Post description, which will be displayed on the article card on the homepage
image: ./assets/cover.jpg
tags: [Tag1, Tag2]
category: Category Name
draft: false
---
```

## 📦 Build & Deployment

Build the static website:

```bash
pnpm build
```

Preview the build result:

```bash
pnpm preview
```

## 📋 Available Commands

| Command                  | Description                                  |
|:-------------------------|:---------------------------------------------|
| `pnpm dev`               | Start the development server at `localhost:4321` |
| `pnpm build`             | Build the production site to the `./dist/` directory |
| `pnpm preview`           | Preview the build result locally before deployment |
| `pnpm new-post <filename>` | Create a new post                              |
