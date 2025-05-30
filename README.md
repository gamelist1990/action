# Resource Pack Converter

このリポジトリは、GitHub Issuesを使用してMinecraftのリソースパックを自動変換するためのGitHub Actionsワークフローを提供します。

## 使い方

1. このリポジトリに新しいIssueを作成します。**タイトルに「build」という単語を含めてください**
2. Issueコメントに変換したいリソースパックファイルのURLのみを記述するか、Markdown形式のリンク（例：`[ファイル名](URL)`）を使用してください
3. 変換対象のファイルは.zipまたは.mcpack形式のリソースパックである必要があります
4. GitHub Actionsが自動的に実行され、McEncryptorを使用してファイルを変換します
5. 変換が完了すると、Issueにラベル「converted」が追加され、変換されたファイルのダウンロードリンクが提供されます

### コメント例

**例1: URLのみの場合**
```
https://github.com/user-attachments/files/12345678/my_resource_pack.zip
```

**例2: Markdown形式の場合**
```
[my_resource_pack.zip](https://github.com/user-attachments/files/12345678/my_resource_pack.zip)
```

## 注意事項

- 変換されたファイルは7日間のみ保存されます
- 大きなファイルの場合、処理に時間がかかる場合があります
- このツールはMinecraftのリソースパック専用です

## 技術的な詳細

このリポジトリは以下のコンポーネントを使用しています：

- GitHub Actions：自動処理のためのワークフロー
- McEncryptor：リソースパックの変換ツール

## ライセンス

このプロジェクトのライセンスについては、LICENSEファイルを参照してください。
