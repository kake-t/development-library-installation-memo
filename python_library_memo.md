# python用ライブラリメモ

## 前提

OS: Windows11

## Scoop

windowsのパッケージ管理ツールpipxをインストールするのに使う

### インストール方法

powershellで以下を実行

```sh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## pipx

pythonのコマンドツールをインストールするのに使用

### インストール方法

```sh
scoop install pipx
pipx ensurepath
```

## pyenv-win

pythonバージョンの管理ツール [公式](https://github.com/pyenv-win/pyenv-win)

<!-- ## Rye

pyenvと競合したので一旦見送る

pythonプロジェクト管理用

### インストール方法

公式サイトからwindows用インストーラーをダウンロードする。

[https://rye.astral.sh/](https://rye.astral.sh/)

### 使い方

#### プロジェクト作成

```sh
rye init
```

#### 新しいバージョンのpython追加

```sh
rye fetch <version>
```

#### プロジェクトのpythonバージョンを変える

`.python-version`のバージョンを変える

```sh
rye fetch
```

#### ライブラリ追加

```sh
rye add <library>
```

開発用ライブラリ追加

```sh
rye add --dev <library>
```

#### ライブラリ同期

```sh
rye sync
``` -->
