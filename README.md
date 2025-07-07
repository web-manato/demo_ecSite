# ECサイトデモページ

## 概要

このプロジェクトは、写真家「山田太郎（YAMADA TARO）」のプロフィールサイトのデモページをベースにしたECサイトのデモです。レスポンシブデザインに対応し、モダンな UI/UX を提供します。

## 特徴

-   **レスポンシブデザイン**: PC・タブレット・スマートフォンに対応
-   **モダンなアニメーション**: GSAP を使用したスムーズなアニメーション
-   **セマンティック HTML**: アクセシビリティに配慮したマークアップ
-   **SASS/SCSS**: 効率的な CSS 管理（@use 構文使用）
-   **お問い合わせフォーム**: PHP を使用した機能的なフォーム（※本リポジトリにはPHPは含まれていません）

## 技術スタック

### フロントエンド

-   **HTML5**: セマンティックなマークアップ
-   **CSS3/SASS**: モダンなスタイリング（@use 構文使用）
-   **JavaScript (ES6+)**: モジュール形式でのインタラクティブ機能
-   **GSAP**: アニメーションライブラリ

### フォント

-   **Lora**: 英語テキスト用
-   **Noto Serif JP**: 日本語テキスト用

## プロジェクト構造

```
demo_ecSite/
├── index.html                # メインページ
├── product.html              # 商品一覧ページ
├── 404.html                  # 404エラーページ
├── css/                      # コンパイル済みCSS
│   ├── styles.css            # メインCSS
│   ├── styles.css.map        # ソースマップ
│   ├── styles.min.css        # 圧縮版CSS
│   └── styles.min.css.map    # 圧縮版ソースマップ
├── sass/                     # SASS/SCSSファイル
│   ├── styles.scss           # メインSASSファイル（@use構文）
│   ├── _variable.scss        # 変数定義
│   ├── _mixin.scss           # ミックスイン
│   ├── _header.scss          # ヘッダー関連スタイル
│   ├── _footer.scss          # フッター関連スタイル
│   ├── _common.scss          # 共通スタイル
│   ├── _index.scss           # メインページスタイル
│   ├── _product.scss         # 商品ページスタイル
│   ├── _error.scss           # エラーページスタイル
│   └── reset.css             # リセットCSS
├── js/                       # JavaScriptファイル（ES6モジュール）
│   ├── main.js               # メインJSファイル
│   ├── hamburger.js          # ハンバーガーメニュー
│   └── fadeIn.js             # フェードインアニメーション
├── img/                      # 画像ファイル（最適化済み）
│   └── ...                   # 各種PC/SP/商品画像・ロゴ等
```

## セクション構成

1. **ヘッダー**: ナビゲーションメニュー（ハンバーガーメニュー対応）
2. **キービジュアル**: メインビジュアルとキャッチコピー
3. **プロフィール**: 写真家の紹介
4. **プロダクト**: 販売作品集
5. **ワークス**: 作品ギャラリー
6. **アワード**: 受賞歴
7. **フォトスクール**: スクール情報
8. **お問い合わせ**: コンタクトフォーム
9. **フッター**: サイト情報

## セットアップ

### 前提条件

-   Web サーバー（Apache/Nginx）
-   PHP 7.4 以上（※本リポジトリにはPHPは含まれていません）
-   Node.js（SASS コンパイル用）

### インストール手順

1. リポジトリをクローン

```bash
git clone [repository-url]
cd demo_ecSite
```

2. 依存関係のインストール（SASS コンパイル用）

```bash
npm install -g sass
```

3. SASS ファイルのコンパイル

```bash
sass sass/styles.scss css/styles.css --style compressed
```

4. Web サーバーでプロジェクトを公開

### 開発用コマンド

SASS ファイルの監視（自動コンパイル）:

```bash
sass --watch sass:css
```

## カスタマイズ

### 画像の変更

-   `img/` フォルダ内の画像ファイルを置き換え
-   ファイル名は既存の命名規則に従ってください

### 色やフォントの変更

-   `sass/_variable.scss` で変数を編集
-   `sass/_mixin.scss` で共通スタイルを編集

### コンテンツの変更

-   `index.html` や `product.html` の各セクション内のテキストを編集
-   画像の alt 属性も適切に更新してください

## ブラウザ対応

-   Chrome (最新版)
-   Firefox (最新版)
-   Safari (最新版)
-   Edge (最新版)
-   Internet Explorer 11 以上

## ライセンス

このプロジェクトはデモ用です。商用利用の際は適切なライセンスを確認してください。

## 作者

まなと

## 更新履歴

詳細な更新履歴は[CHANGELOG.md](./CHANGELOG.md)をご確認ください。 