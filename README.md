# Claude Code Agents for MEO Shop

> 店舗ビジネス（飲食・美容・治療院・小売）のひとりオーナー向け、Claude Code サブエージェント集。
> MEO・口コミ管理・地域マーケ・SNS 運用・カスタマージャーニー・年間販促を AI で加速する。

[English version below](#english)

---

## 🎯 これは何か

[Claude Code](https://docs.claude.com/en/docs/claude-code/overview) で店舗ビジネスの集客・運営判断を補助する、6 つの専門エージェント定義集です。

ベースの C-Suite エージェント（CFO・CMO・CRO 等）と組み合わせて使うことを想定しています。

```
あなた: @meo-strategist
        Google ビジネスプロフィールの写真を増やしたいが、何から撮るべき？

meo-strategist:
        外観 → 内観 → 主力メニューの順で揃えるのが基本です。
        御店の業態と現在の写真構成を踏まえると、まず「夜の外観」と…
```

## 👥 含まれる 6 エージェント

| エージェント | 主な相談内容 |
|---|---|
| **meo-strategist** | Google ビジネスプロフィール最適化・MEO 戦略・写真戦略 |
| **review-responder** | 口コミ返信・ネガティブレビュー対応・口コミ獲得施策 |
| **local-marketer** | 商圏分析・地域 SEO・チラシ/ポスティング・地域連携 |
| **sns-operator** | Instagram・LINE 公式・X 等の店舗 SNS 運用設計 |
| **customer-journey** | 来店動線・予約導線・再来店設計・LTV 最大化 |
| **seasonal-planner** | 年間販促カレンダー・季節企画・繁閑差対策 |

## 🚀 クイックスタート

### 前提：ベースの C-Suite エージェント集を導入

このパックは以下と組み合わせて使います：

- [claude-code-c-suite-agents](https://github.com/OceansCreative/claude-code-c-suite-agents)（CFO・CMO・CRO 等の汎用 13 エージェント）

ベースのリポジトリの `.claude/` ディレクトリと `CLAUDE.md.template` を先に導入してください。

### このパックの追加

```bash
git clone https://github.com/OceansCreative/claude-code-agents-meo-shop.git
cd /path/to/your/project

# 6 つの店舗特化エージェントを追加
cp claude-code-agents-meo-shop/.claude/agents/*.md .claude/agents/

# 店舗ビジネス特化の CLAUDE.md テンプレートを使う場合（推奨）
cp claude-code-agents-meo-shop/CLAUDE.md.template ./CLAUDE.md
```

### CLAUDE.md を埋める

業種別の記入例を [`examples/`](./examples/) に用意しています：

- [飲食店（居酒屋）](./examples/restaurant/CLAUDE.md)
- [美容室](./examples/beauty-salon/CLAUDE.md)
- [治療院（鍼灸院）](./examples/treatment-clinic/CLAUDE.md)

## 💡 設計思想

このパックは「**ひとり店主**」を主な想定読者として作っています。

- **法令遵守を埋め込む**：飲食店なら食品衛生法、美容なら美容師法、治療院ならあはき法、共通して景品表示法・個人情報保護法を必ず意識する
- **来店が最終目標**：Web 集客は手段であり目的ではない。SNS フォロワー数より来店転換率を重視
- **ひとりで続けられる頻度**：派手なバズより継続可能な定期運用を優先
- **常識的な範囲での提案**：ステマ規制・口コミ操作・ガイドライン違反などには明確に NO

## 📜 ライセンス

MIT License - [LICENSE](./LICENSE) を参照。

自由に fork ・改変・商用利用してください。改善案やプルリクエスト歓迎です。

## 🙋 つくったひと

開発・メンテナンス：**池田和司（[OceansBase](https://oceans-base.com)）**

[OceansBase](https://oceans-base.com) は島根県を拠点とする個人事業屋号で、受託開発・IT コンサル・コンテンツ制作を行っています。

---

<a id="english"></a>

# Claude Code Agents for MEO Shop (English)

> A specialized agent pack for solo store-business owners (restaurants, salons, treatment clinics, retail). Use alongside [claude-code-c-suite-agents](https://github.com/OceansCreative/claude-code-c-suite-agents) to accelerate local marketing decisions with AI.

## Six Specialized Agents

- **meo-strategist** – Google Business Profile / local SEO
- **review-responder** – Review reply strategy across platforms
- **local-marketer** – Trade area analysis, flyers, local partnerships
- **sns-operator** – Instagram, LINE, X for store businesses
- **customer-journey** – From discovery to repeat visit
- **seasonal-planner** – Annual promotional calendar, seasonal campaigns

## Quickstart

```bash
git clone https://github.com/OceansCreative/claude-code-agents-meo-shop.git
cp claude-code-agents-meo-shop/.claude/agents/*.md /path/to/your/project/.claude/agents/
cp claude-code-agents-meo-shop/CLAUDE.md.template /path/to/your/project/CLAUDE.md
```

## License

MIT - free to fork, modify, and use commercially.

## Author

Maintained by **Kazushi Ikeda** ([OceansBase](https://oceans-base.com)) — solo IT consulting practice in Shimane, Japan.
