# vscode 設定

## 前提

- OS: Windows
- コマンドは powershell で実行する

## ファイル説明

| ファイル名     | 説明                           |
| -------------- | ------------------------------ |
| extensions.txt | 拡張機能のエクスポートファイル |
| settings.json  | ユーザ設定ファイル             |

## 設定手順

### 拡張機能のエクスポート

```sh
code --list-extensions > extensions.txt
```

### 拡張機能のインポート

```sh
cat extensions.txt | ForEach-Object { code --install-extension $_ }
```

### ユーザ設定

`settings.json`を vscode ユーザ設定にコピペしてください。
