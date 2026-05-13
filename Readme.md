# mu-workspace

`mu-workspace` は、下記のプロジェクトをまとめて管理するワークスペースです。
- `mmemo`
- `sail`
- `mu-ui-lib`

## 開き方

VS Code では `mu.code-workspace` を開いてください。

- ルート
- `mmemo`
- `sail`
- `mu-ui-lib`

をまとめて開けるので、プロジェクト間を行き来しやすくなります。

## セットアップ

初回はルートで依存関係を入れます。

```bash
yarn install
```

## 補足

- このワークスペースは Yarn 1 系を前提にしています。
- Node.js は `>=24.13.1 <25` を想定しています。
- 各フロントエンドの依存関係は `mmemo/front` と `sail/front` の workspace として管理しています。
- 共有 UI は `mu-ui-lib` に置き、各フロントエンドから参照します。

## 関連プロジェクトのリポジトリ

```bash
git clone https://github.com/multios12/mmemo.git
git clone https://github.com/multios12/ops-front.git
git clone https://github.com/multios12/sail.git
git clone https://github.com/multios12/mu-ui-lib.git
```
