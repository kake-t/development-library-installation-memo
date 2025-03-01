# python用ライブラリメモ

## 前提

OS: Windows11

## Rye

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
```
