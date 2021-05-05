### 雛形作成

- `yarn create next-app .`

### ディレクトリ構成の変更

- `mkdir src && \ mv pages/ src/pages & \ mv styles/ src/styles`

### TypeScript の導入

- `yarn add -D typescript @types/react @types/react-dom @types/node`
- `tsconfig.json` , `next-env.d.ts` を作成
- `yarn dev` で tsconfig.json に書き込みを行う

## コードの自動整形設定

- vscode のプラグインから `prettier` と `ES7 React` のアドオンを追加
- eslint prettier 関連のパッケージをインストール（windows の場合はコマンドが違うかもしれません）
  - `yarn add -D eslint prettier eslint-config-prettier`
  - `yarn add -D @typescript-eslint/{parser,eslint-plugin}`
  - `yarn add -D eslint-plugin-{react,react-hooks}`
- `.eslintrc.json` の作成
- `.prettierrc.json` の作成 （詳しい設定については後ほど）
- package.json に`"eslint:fix": "eslint . --ext .js,.ts,.jsx,.tsx --fix"`および`"prettier:fix": "prettier --write ."`を追加
- `yarn prettier:fix`を実行

## Readux Toolkit の導入

- `yarn add redux react-redux @reduxjs/toolkit redux-logger`
- `yarn add -D @types/react-redux @types/redux-logger`

## 参考ページ

- [参考](https://zenn.dev/higa/articles/d7bf3460dafb1734ef43#%E6%8A%80%E8%A1%93%E9%81%B8%E5%AE%9A)
