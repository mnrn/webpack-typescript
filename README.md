# Webpack + Babel + TypeScript のテンプレート

webpackとbabelを組み合わせた場合のテンプレートになります。

## 依存関係

package.jsonにある通りです。

```terminal
npm init -y

# Webpack関連
npm install webpack webpack-cli webpack-merge --save-dev

# 開発用サーバー
npm install webpack-dev-server --save-dev

# TypeScript関連
npm install typescript ts-loader --save-dev
```

## ディレクトリ構成

```txt
develop-root/
  ├ src/
  │   ├ components/
  │   └ index.ts 
  ├ dist/
  │   ├ js/
  │   └ index.html
  ├ tsconfig.json
  ├ webpack.common.js
  ├ webpack.dev.js
  └ webpack.prod.js
```

## 使い方

```terminal
# 開発用ビルド
npm run build:dev

# 開発用サーバー立ち上げ
npm run serve

# 本番用ビルド
npm run build
```
