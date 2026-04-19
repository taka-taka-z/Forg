# Forg v1.0.0 Release Notes

**Release Date**: 2026-04-19
**Codename**: Ztelier Integration

---

## エグゼクティブサマリ

Forg v1.0.0 は、**Ztelier傘ブランド配下の正式版**として再出発するリリースです。
v4系までに蓄積した「組織摩擦の定量化」という思想を、Ztelier Common Kit 統合・Suggestion層搭載・経営層サマリ完備という3本柱で完成形にしました。

## v1.0.0 の3本柱

### 1. Ztelier Common Kit 統合

MAAZ / Endeavor など他アセスメントツールとの連携を前提とした共通設計を採用。

- Ztelierブランドカラー（Primary #246CF7 / Navy #001744 / Sage #7BA05B）を適用
- 共通JSONスキーマ（`ztelier-context-schema.json`）で結果を出力
- Architecture Workshop の一連のアセスメントツールチェーンに組み込み可能

### 2. Suggestion層（4パターン×優先アクション）

診断結果のパターン分類に応じて、確立されたChange Managementフレームワークを参照元とする優先アクションを自動提示。

| パターン | 診断の特徴 | 参照フレーム |
|---|---|---|
| Leadership Gap | 経営層の発信が現場に届かない | Kotter Step 1-2（Urgency） |
| Execution Silo | 戦略は明確だが実行が分断 | Kotter Step 5-6（Empowerment） |
| Change Resistance | 変革への個人的抵抗が強い | ADKAR（Awareness / Desire） |
| Legacy Anchor | レガシー負債が意思決定を束縛 | Kotter Step 3-4（Vision） |

「なんとなく進まない」を、議論可能な数字と具体的な次の一手に変換します。

### 3. 経営層サマリ

ボトルネック・想定機会損失・推奨アクションを1画面に集約。CxO層へのレポーティングにそのまま転用できる出力を実装しました。

## 旧バージョンからの重要な変更点

### バージョン体系のリセット

v4.3.0 相当の機能を v1.0.0 として再リリースしました。Ztelier配下の正式版という位置づけです。

- 旧リポジトリの v4.x タグは参照用として保持
- v1.0.0 以降は Semantic Versioning に厳密に準拠

### 設問の視覚表現

山根さん（0-WAN）からのフィードバックを反映し、分子側（S / L）は「荷物」、分母側（C / L'）は「エンジン出力」のメタファーで回答時の方向感を直感化しました。

### 想定被害額の根拠明示

BVA実施済み顧客との矛盾回避のため、算出ロジック（日商×14日×20% + 2億円）を画面に明示。「参考値」である旨を注釈に追加しました。

## 互換性

| 項目 | 互換性 |
|---|---|
| 診断ロジック | v4系と互換（F_org計算式は変更なし） |
| 設問内容 | v4.1系以降と互換（19問構成） |
| JSONエクスポート | 共通スキーマに移行。旧形式は読込時に自動変換 |
| ブラウザ | Chrome / Edge / Safari（最新版） |

## 次期バージョンの予定

- **v1.1.0**: 業種別ベンチマーク機能（製造・金融・公共など）
- **v1.2.0**: 多言語対応（英語版）
- **将来**: AW現場データに基づくSuggestion層の精度向上

## 謝辞

本リリースは、Architecture Workshop 250社以上の現場経験と、山根さん（0-WAN）をはじめとする実戦ユーザーからのフィードバックによって成立しました。「一緒にツールを育てる」という姿勢に応えてくれたすべての方に感謝します。

## ダウンロード

- [index.html](./index.html) をブラウザで開くだけ
- オフライン動作・データ送信なし

## リンク

- [README](./README.md)
- [操作ガイド](./docs/OPERATION_GUIDE.md)
- [変更履歴](./CHANGELOG.md)
- [Ztelier Common Kit](https://github.com/taka-taka-z/ztelier-common-kit)

---

**Takayoshi Takaoka**
Evangelist & Transformation Architect, Zscaler Japan
[LinkedIn](https://www.linkedin.com/in/takayoshi-takaoka-6001742/)

*本ツールはZscaler公式製品ではありません。個人研究・実務経験に基づき開発しました。*
