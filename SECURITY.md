# Security Policy

## サポート対象 / Supported Versions

最新の `main` ブランチおよび最新の GitHub Release のみをサポートします。
Only the latest `main` branch and the latest GitHub Release are supported.

| Version | Supported |
|---------|-----------|
| latest (main / latest release) | ✅ |
| older releases | ❌ |

## このリポジトリの性質 / Nature of this repository

このリポジトリは **Claude Code 用のサブエージェント定義（プロンプト集）** であり、実行可能コードや依存ライブラリを含みません。一般的なソフトウェア脆弱性（メモリ破壊、SQL インジェクション、依存関係の CVE 等）は本質的に発生しません。

This repository contains **Claude Code subagent definitions (prompts)** with no executable code or library dependencies. Conventional software vulnerabilities (memory corruption, SQL injection, dependency CVEs, etc.) are not applicable.

## セキュリティ上の懸念とみなす範囲 / What we consider security issues

以下のような問題はセキュリティ報告として扱います。

The following are treated as security reports:

- **悪用可能なプロンプト** — エージェントを通じて Claude に意図せず有害な出力をさせるプロンプト構造 / Prompt structures that could induce Claude to produce unintended harmful output
- **法令違反を促す内容** — 景品表示法のステマ規制、薬機法、あはき法、美容師法、食品衛生法などに違反する助言を生成しうる定義 / Definitions that could generate advice violating Japanese laws (advertising, cosmetology, medical, food safety, etc.)
- **個人情報・機微情報の漏洩** — リポジトリ内に第三者の個人情報や認証情報が含まれている場合 / Personal data or credentials accidentally committed to this repository
- **ライセンス違反** — 第三者の著作物の不適切な転載 / Improper copying of third-party copyrighted material

## 報告方法 / How to report

**公開 Issue は使わないでください。** 以下のいずれかの方法で報告をお願いします。

**Please do NOT open a public Issue.** Use one of the following channels:

1. **メール / Email**: `system@oceans-creative.com`
2. **GitHub Security Advisories（推奨 / preferred）**: [Report a vulnerability](https://github.com/OceansCreative/claude-code-agents-meo-shop/security/advisories/new)

## 対応プロセス / Response process

| ステップ / Step | 想定期間 / Target time |
|---|---|
| 受領確認 / Acknowledgement | 7 営業日以内 / within 7 business days |
| 初期評価 / Initial assessment | 14 営業日以内 / within 14 business days |
| 修正および公開 / Fix and disclosure | 重大度に応じて調整 / depends on severity |

報告者の情報は本人の同意なく公開しません。修正のリリース時に、希望があればクレジットを記載します。

Reporter information will not be disclosed without consent. Credit will be given upon request when the fix is released.

## 範囲外 / Out of scope

- Claude Code 本体や Claude API の脆弱性 → [Anthropic](https://www.anthropic.com/) へ報告してください / Report Claude Code or Claude API vulnerabilities to [Anthropic](https://www.anthropic.com/) directly
- ユーザー自身の `CLAUDE.md` 内に記載した機微情報の漏洩（このリポジトリのライセンスでは個別ユーザーの利用環境は対象外）/ Leaks from user-customized `CLAUDE.md` files outside this repository
