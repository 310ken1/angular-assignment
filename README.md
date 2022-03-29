# Angular

## １週目：Angular を知ろう

以下を読もう

- [Angular とは何か？](https://angular.jp/guide/what-is-angular)
- [TypeScript の特徴](https://typescriptbook.jp/overview/features)
- [Node.js とは](https://typescriptbook.jp/tutorials/setup)

## ２週目：開発環境の構築

公式サイトの[セットアップ](https://angular.jp/guide/setup-local)に従えば良いが、以下補足。

### アプリ のインストール

- Visual Studio Code

  [winget](https://docs.microsoft.com/ja-jp/windows/package-manager/winget/)でインストールする場合

  ```batch
  winget install -e --id Microsoft.VisualStudioCode
  ```

- Git

  ```batch
  winget install -e --id Git.Git
  ```

- Node.js

  バージョン管理ツールを使うと、バージョン違いの Node.js を共存させる場合に管理しやすい

  - [fnm](https://github.com/Schniz/fnm)
  - [volta](https://github.com/volta-cli/volta)
  - [nvs](https://github.com/jasongin/nvs)

  fnm の場合

  ```batch
  fnm use v16.14.2
  ```

### Angular CLI のインストール

```batch
npm install -g @angular/cli
```

-g オプションについて
: -g オプションを付ける事で、グローバルインストールされる
ng コマンドを、どこからでも実行できるようになる

## ３週目：プロジェクトの作成と実行

1. プロジェクトの作成

   ```batch
   ng new <プロジェクト名>
   ? Would you like to add Angular routing? Yes
   ? Which stylesheet format would you like to use? SCSS
   ```

2. Node.js のバージョン保存(fnm 利用時)

   ```batch
   node --version > .node-version
   ```

3. 実行
   ```batch
   ng serve -o
   ```
