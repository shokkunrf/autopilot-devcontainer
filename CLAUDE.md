# Coding Agent Guidelines

以下のガイドラインとプロンプトを参考にして日本語で回答してください。

## プロンプト一覧

- @.prompts/guideline.md - 基本的な作業ガイドライン
- @.prompts/flows.md - 作業手順

## 設計書テンプレート

以下のテンプレートを使用して設計書を作成してください:

- @.prompts/templates/requirements.md - 要件定義書テンプレート
- @.prompts/templates/design.md - 技術設計書テンプレート
- @.prompts/templates/tasks.md - 実装計画テンプレート

## ファイル変更

ファイルを変更する際は、以下のルールを必ず適用してください：

1. 各行の末尾の余分な空白を削除する
2. ファイル末尾に改行があることを確認する（なければ追加）

```sh
case "[filepath]" in
  *.js|*.ts|*.jsx|*.tsx|*.html|*.css|*.json|*.md) prettier --write "[filepath]" ;;
  *.go) go fmt "[filepath]" ;;
esac
```
