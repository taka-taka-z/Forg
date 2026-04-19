# Forg — 組織摩擦係数診断ツール

> 「なぜゼロトラスト導入はいつも途中で止まるのか」
> その答えは技術ではなく、組織の中にある。

[![Version](https://img.shields.io/badge/version-1.0.0-246CF7)](https://github.com/taka-taka-z/forg/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-7BA05B)](./LICENSE)
[![Part of Ztelier](https://img.shields.io/badge/part_of-Ztelier-001744)](https://github.com/taka-taka-z/ztelier-common-kit)

## これは何か

Forg（フォルグ）は、企業のゼロトラスト推進を阻む**組織摩擦**を定量的に可視化するブラウザベースの診断ツールです。独自指標「組織摩擦係数 F_org」をベースに、停滞理由の言語化と優先アクションを即座に導出します。

## 主な機能

- **F_org スコア算出** — 4変数（Structure / Legacy / Crisis / Leadership）から摩擦係数を計算
- **矛盾検出ロジック** — 回答間の整合性を自動チェック（例：「変革意志は高いがPoC失敗を許容しない」）
- **アーキタイプ診断** — 組織を4象限マトリクス（加速型 / 停滞型 / 膠着型 / 偽装型）で分類
- **Suggestion層** — 4パターンごとにKotter / ADKARを参照元とした優先アクションを提示
- **経営層サマリ** — ボトルネック・想定機会損失・推奨アクションを1画面に集約
- **PDF出力** — 報告書フォーマットで保存可能

## 使い方

ブラウザで `index.html` を開くだけ。インストール不要・オフライン動作・データ送信なし。

詳細は[操作ガイド](./docs/OPERATION_GUIDE.md)を参照してください。

## 設計思想

Forgは**Ztelier**（ゼロトラスト推進のためのアセスメント・ツールチェーン）の一部として設計されています。単独利用も可能ですが、[Ztelier Common Kit](https://github.com/taka-taka-z/ztelier-common-kit)と組み合わせることで、MAAZ / Endeavor など他ツールとの結果連携（共通JSONスキーマ）が可能になります。

## 対象ユーザー

ゼロトラスト導入を検討・推進中のCISO・セキュリティアーキテクト・DX推進担当者。Architecture WorkshopのAS-ISセッションでのファシリテーションツールとしても活用可能です。

## ライセンス

[MIT License](./LICENSE)

## 開発者

**Takayoshi Takaoka**
Evangelist & Transformation Architect, Zscaler Japan
[LinkedIn](https://www.linkedin.com/in/takayoshi-takaoka-6001742/)

## ドキュメント

- [操作ガイド](./docs/OPERATION_GUIDE.md)
- [変更履歴](./CHANGELOG.md)
- [v1.0.0 リリースノート](./RELEASE_NOTES_v1.0.0.md)

---

*本ツールはZscaler公式製品ではありません。個人研究・実務経験に基づき開発しました。診断結果は組織変革の議論を促すための参考値であり、厳密な経営判断には追加分析を推奨します。*
