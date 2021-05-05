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
