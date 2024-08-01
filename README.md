## What is this?

Bun + Nuxt3 で作られた会社でもバレずに使えるかもしれない Google 検索風のクライアントです

## 自分用メモ

Nuxt3 のディレクトリ構成は以下を参考に

https://zenn.dev/r0227n/articles/nuxt3_directory_structure_memo

- `.nuxt`: Nuxt.js が開発モードで起動されたときに自動的に生成されるディレクトリ。ビルドされたアプリケーションのファイルが格納されます。
- `.output`: nuxt generate コマンドによって静的に生成されたサイトのファイルが出力されるディレクトリ。
- `assets`: スタイルシート、画像、フォントなどの静的なアセットを格納するディレクトリ。
- `components`: 再利用可能な Vue コンポーネントを格納するディレクトリ。これらのコンポーネントは自動的にインポートされ、どこからでも使用できます。
- `composables`: Vue 3 の Composition API を使用した再利用可能なロジック（composable）を格納します。アプリケーション内で自動で import される。
- `content`: マークダウンファイルや CSV ファイルなどのコンテンツを格納するディレクトリ。
- `layouts`: アプリケーションのレイアウトを定義するディレクトリ。レイアウトはページの共通部分（例えばヘッダーやフッター）を定義するために使用されます。
- `middleware`: アプリケーションのミドルウェアを定義するディレクトリ。ミドルウェアは、ページやレイアウトがレンダリングされる前に実行されるカスタム関数です。
- `modules`: Nuxt.js のモジュールを格納するディレクトリ。モジュールは、Nuxt.js のコア機能を拡張するためのコードを含む JavaScript ファイルです。
- `node_modules`: プロジェクトの依存関係を格納するディレクトリ。npm install または yarn install コマンドを実行すると、このディレクトリに依存関係がインストールされます。
- `pages`: ルーティングとページコンポーネントが自動的に生成されます。各 Vue ファイルは対応するルートとなります。
- `plugins`: Vue.js のプラグインを格納するディレクトリ。これらのプラグインは、Nuxt.js がインスタンス化される前に実行されます。
- `public`: 静的ファイル（画像、スタイルシート、ロボット.txt など）を格納します。これらのファイルはそのままのパスで公開されます。
- `server`: サーバーサイドのロジックを格納します。このディレクトリ内に配置したファイルはサーバーサイドで実行され、API エンドポイントとして利用できます。
- `utils`: ユーティリティ関数など、プロジェクト全体で使用する JavaScript のヘルパー関数を格納します。

## インストール

先に Bun をインストールしてください

https://bun.sh/docs/installation

```bash
git clone https://github.com/shibaTT/phantom-social-client.git
cd phantom-social-client
bun install
```

## ローカル確認

引数で bun を渡さないと Node で起動してしまうみたいです

```bash
bun --bun run dev
```

## ビルド

```bash
bun run build
```

## プレビュー

```bash
npm run preview
```