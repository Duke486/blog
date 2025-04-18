# 個人的な技術ブログ

Astroで作られた個人的な技術ブログです。主に技術学習とACGN関連の技術記事、チュートリアル、経験を共有します！

## 🔧 技術スタック

- 構築フレームワーク: [Astro](https://astro.build)
- テーマ: [Fuwari](https://github.com/saicaca/fuwari)をベースにカスタマイズ

## 🚀 ローカルで実行する

1. このリポジトリをクローンします

   ```bash
   git clone <your-repo-url>
   cd AstroBlog
   ```

2. 依存関係をインストールします

   ```bash
   pnpm install
   pnpm add sharp
   ```

3. 開発サーバーを起動します

   ```bash
   pnpm dev
   ```

4. 新しい記事を作成します

   ```bash
   pnpm new-post <記事ファイル名>
   ```

   それから posts ディレクトリに新しく作成された記事を編集します

## 📝 記事のフォーマット

記事はMarkdown形式を使用します。ファイルの先頭にfrontmatter情報を追加する必要があります:

```yaml
---
title: 記事のタイトル
published: 2025-04-10
description: 記事の説明です。ホームページの記事カードに表示されます
image: ./assets/cover.jpg
tags: [タグ1, タグ2]
category: カテゴリ名
draft: false
---
```

## 📦 ビルドとデプロイ

静的ウェブサイトをビルドします:

```bash
pnpm build
```

ビルド結果をプレビューします:

```bash
pnpm preview
```

## 📋 利用可能なコマンド

| コマンド                  | 説明                                          |
|:-------------------------|:---------------------------------------------|
| `pnpm dev`               | 開発サーバーを起動します。アドレスは`localhost:4321`です |
| `pnpm build`             | 本番サイトを`./dist/`ディレクトリにビルドします        |
| `pnpm preview`           | デプロイ前にローカルでビルド結果をプレビューします            |
| `pnpm new-post <ファイル名>` | 新しい記事を作成します                              |
