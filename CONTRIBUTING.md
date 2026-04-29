# Contributing

このプロジェクトへの貢献を歓迎します。エージェント追加・改善提案・誤字修正、どれも大歓迎です。

## バグ報告・改善提案

[Issues](https://github.com/OceansCreative/claude-code-agents-meo-shop/issues) で報告してください。以下を含めると対応がスムーズです。

- 使用していた Claude Code のバージョン
- 該当エージェント名（例：`meo-strategist`）
- 期待した挙動 / 実際の挙動
- （可能なら）再現できる `CLAUDE.md` の抜粋

## プルリクエスト

1. 大きな変更（新エージェント追加・既存エージェントの方針変更）は、先に Issue を立てて方針を相談してください。
2. ブランチ名は `feat/xxx` `fix/xxx` `docs/xxx` のいずれかを推奨します。
3. エージェント定義を追加・変更する場合：
   - frontmatter に `name` `description` `model` を必ず記載
   - 法令・ガイドライン違反を促す記述は不可（景品表示法のステマ規制、薬機法、あはき法、美容師法、食品衛生法など）
   - 業種例を追加する場合は `examples/<業種名>/CLAUDE.md` に配置

## コミットメッセージ

[Conventional Commits](https://www.conventionalcommits.org/) を推奨します。

- `feat: ` 新機能・新エージェント
- `fix: ` バグ修正・記述ミス修正
- `docs: ` ドキュメント更新
- `chore: ` その他

## 行動規範

このプロジェクトの参加者は [Code of Conduct](./CODE_OF_CONDUCT.md) に従うものとします。

## ライセンス

PR を送ることで、その成果物が [MIT License](./LICENSE) で配布されることに同意したものとみなします。

---

# Contributing (English)

Contributions welcome — new agents, improvements, typo fixes, all appreciated.

## Reporting issues

Open an [Issue](https://github.com/OceansCreative/claude-code-agents-meo-shop/issues) and include:

- Claude Code version
- Affected agent name
- Expected vs. actual behavior
- A minimal `CLAUDE.md` snippet that reproduces the issue, if applicable

## Pull requests

- Open an issue first for non-trivial changes (new agents, behavioral overhauls).
- Branch names: `feat/xxx`, `fix/xxx`, `docs/xxx`.
- New agent definitions must include `name`, `description`, `model` in frontmatter, and must not encourage violations of advertising, cosmetology, or medical laws applicable to Japanese store businesses.
- Place new industry examples under `examples/<industry-name>/CLAUDE.md`.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/): `feat: ` / `fix: ` / `docs: ` / `chore: `.

## Code of Conduct

All participants are expected to follow our [Code of Conduct](./CODE_OF_CONDUCT.md).

## License

By submitting a PR you agree your contribution is licensed under MIT.
