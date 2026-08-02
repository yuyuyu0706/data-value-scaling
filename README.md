# データ活用スケーリング計画

> **データ資本から事業価値への変換効率を捉え、小規模なユースケースを継続利用・拡大・横展開・共通化へ育てるための計画です。**

このリポジトリでは、Databricks を用いたデータ活用を事業価値につなげるための共通言語、主要指標モデル、ポートフォリオ管理の考え方を段階的に整備します。現在は **Phase 0（プロジェクト管理環境の整備）** です。

本 README は、プロジェクトの全体像と成果物への入口です。背景、定義、対象範囲、基本原則、成功状態の詳細は、正本である[プロジェクト憲章 Draft v0.1](docs/00_project/charter.md)を参照してください。

## プロジェクト概要

データや分析環境を保有し、ユースケースの数や利用量を増やすだけでは、事業価値が持続的に生まれるとは限りません。本プロジェクトは、ユースケースごとの価値仮説、成果、コスト、リスク、定着状況、学習を捉え、次の投資や改善を判断できる状態を目指します。

小規模なユースケースを削減対象とは考えません。小さな試行を価値発見の入口として尊重し、結果を基に継続、改善、拡大、横展開、共通化、保留、終了を選びます。成功と終了の双方から得たデータ、部品、知識、運用能力を次の試行へ還流させ、価値創出の速度・確度・効率を高めます。

## 中核コンセプトと基本原則

### 4 つの主要概念

| 概念 | このプロジェクトでの捉え方 |
| --- | --- |
| データ資本 | データに加え、品質、基盤、知識、運用能力、権限など、活用を可能にする蓄積 |
| ユースケース | 課題や機会に対し、データを用いて価値仮説を検証・実現する活動の単位 |
| 事業価値 | 売上・利益への寄与、コスト・時間の削減、品質・顧客体験・意思決定の改善、リスク低減などの意味ある変化 |
| スケール | 価値が確認された活用が、定着、対象拡大、横展開、共通化を通じて持続的かつ効率的に価値を増やすこと |

これらを、次の循環として捉えます。

1. データ資本をユースケースへ投入し、小さく価値仮説を検証する。
2. 事業価値、コスト、リスク、利用状況、学習を観測する。
3. 根拠に基づいて次の行動と資源配分を決める。
4. 成果と学習をデータ資本として蓄積し、次のユースケースで再利用する。

判断では、**事業価値を起点にすること**、**規模ではなく価値を伴う成長を目指すこと**、**ユースケース群をポートフォリオとして最適化すること**を重視します。指標や可視化は報告自体を目的とせず、優先順位付けと改善のために用います。また、初期から過度な精度を求めず、得られた事実に合わせて測定とモデルを成熟させます。

## 対象範囲・非対象

### 対象範囲

- データ活用を価値仮説から定着、拡大、横展開、共通化まで一貫して捉える概念
- 価値、投入資源、コスト、リスク、成熟度、利用・定着、学習に関する主要指標モデル
- 個別ユースケースとユースケース群を扱うポートフォリオ管理
- データ資本から事業価値への変換と、再利用可能な資産の還流の可視化
- 測定結果を資源配分や継続・改善・拡大・保留・終了の判断につなげる運用仮説

### 非対象

- 規模、利用量、データ量だけを理由にしたユースケースの一律削減
- 活動件数やデータ量の増加自体を成果とすること
- データの正式な会計資産評価や、会計・予算・人事等の制度策定
- Databricks の個別機能、アーキテクチャ、実装標準の網羅
- すべての事業価値を初期から単一金額や精密な KPI に換算すること
- 個別ユースケースの要件定義、開発、運用の代行

## 主要指標・主要モデル（Draft）

指標体系は後続 Phase で検証・詳細化します。現時点で合意している全体像は次のとおりです。算定式、データソース、測定頻度、目標値は今後定義します。

### 最上位KPI

- **事業価値実現額:** データ活用によって実現した事業価値を捉える
- **価値実現率:** 想定した事業価値に対して、どの程度の価値を実現できたかを捉える
- **データ活用ポートフォリオ収益率:** ユースケース群への投入に対して実現した価値をポートフォリオとして捉える

### KPI領域

| KPI領域 | 主な測定観点の例 |
| --- | --- |
| 価値創出 | 財務効果、時間・品質・顧客体験・意思決定の改善、リスク低減 |
| スケール | 成熟度・定着、継続利用、利用範囲、横展開、共通化 |
| ポートフォリオ | 投入・コスト、期待価値と実績、リスク・持続性、資源配分 |
| 基盤効率 | データ・部品・知識の再利用、品質、運用負荷、価値創出までの時間 |

### 主要モデル

- **データ価値キャッシュフロー:** データ活用への投入から事業価値の実現までの流れを捉える
- **価値実現スコアカード:** 価値創出、スケール、ポートフォリオ、基盤効率を複数の観点から捉える
- **データ活用損益計算書:** データ活用による価値と、その創出に要したコストの関係を捉える
- **データ活用バランスシート:** 蓄積されたデータ資本と、価値創出を支える状態を捉える

これらのモデルは、正式な財務諸表や会計上の資産評価を意味しません。**ユースケース台帳**は主要モデルそのものではなく、各モデルに必要な価値仮説、成果、コスト、リスク、成熟度、利用状況、学習などを管理する成果物として位置付けます。

## ロードマップ概要と現在地（Draft）

Phase の詳細な目的、主要成果物、開始・完了条件、依存関係、引継ぎは、正本である[全体ロードマップ Draft v0.3](docs/00_project/roadmap.md)で管理します。以下は入口としての短い要約です。

| Phase | 方向性 | 状態 |
| --- | --- | --- |
| 0 | プロジェクト管理環境を整備する | **進行中** |
| 1 | [指標モデルの共通言語を定義する](https://github.com/yuyuyu0706/data-value-scaling/issues/36) | 計画中（Lv1 Issue 起票済み） |
| 2 | データ価値キャッシュフローMVPを構築する | Draft |
| 3 | 価値実現スコアカードを構築する | Draft |
| 4 | データ活用損益計算書を構築する | Draft |
| 5 | データ活用バランスシートを構築する | Draft |
| 6 | データ活用スケーリング計画へ統合する | Draft |

現在の Phase と作業の起点は [Phase 0（Issue #1）](https://github.com/yuyuyu0706/data-value-scaling/issues/1)、次に着手する候補 Phase の実行計画は [Phase 1（Issue #36）](https://github.com/yuyuyu0706/data-value-scaling/issues/36)で確認できます。現在の進捗は [GitHub Project](https://github.com/users/yuyuyu0706/projects/6/views/1) と各 Issue で管理し、Phase 間の計画は[全体ロードマップ](docs/00_project/roadmap.md)を参照します。

## 成果物・管理情報

| 情報 | 役割 | 参照先 |
| --- | --- | --- |
| Repository README | プロジェクト概要と主要情報への入口 | 本文書 |
| プロジェクト憲章 | 背景、目的、定義、原則、スコープ、成功状態の詳細 | [`docs/00_project/charter.md`](docs/00_project/charter.md) |
| 全体ロードマップ | Phase 0〜6 の実行順序、成果ゲート、依存関係、引継ぎ | [`docs/00_project/roadmap.md`](docs/00_project/roadmap.md) |
| 文書管理ルール | 情報種別ごとの正本、更新責任、参照・同期ルール | [`docs/00_project/document-governance.md`](docs/00_project/document-governance.md) |
| Repository 構成ガイド | 物理配置、領域の責務境界、構成変更の判断基準 | [`docs/00_project/repository-structure.md`](docs/00_project/repository-structure.md) |
| Issue・Pull Request 管理ルール | Issue 階層、ライフサイクル、関連付け、状態管理 | [`docs/00_project/issue-pr-management.md`](docs/00_project/issue-pr-management.md) |
| Issue テンプレート | Lv1〜Lv4 Issue 起票時の入力補助 | [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/) |
| Pull Request テンプレート | 関連 Issue、変更範囲、確認結果、レビュー観点の入力補助 | [`.github/pull_request_template.md`](.github/pull_request_template.md) |
| 管理文書 | `docs/` 領域の利用案内 | [`docs/README.md`](docs/README.md) |
| 意思決定記録 | `decisions/` 領域の利用案内と現在の運用状態 | [`decisions/README.md`](decisions/README.md) |
| 指標・共通定義 | `definitions/` 領域の利用案内 | [`definitions/README.md`](definitions/README.md) |
| データ | `data/` 領域の利用案内と安全条件 | [`data/README.md`](data/README.md) |
| 分析 | `analytics/` 領域の利用案内 | [`analytics/README.md`](analytics/README.md) |
| GitHub Issues | Phase、成果物、実装作業の計画と完了条件 | [Issues](https://github.com/yuyuyu0706/data-value-scaling/issues) |
| GitHub Project | 現在の重点と進捗の管理 | [Projects](https://github.com/users/yuyuyu0706/projects/6/views/1) |
| Pull Requests | 成果物の変更、レビュー、変更理由の履歴 | [Pull requests](https://github.com/yuyuyu0706/data-value-scaling/pulls) |

上表の各領域 README と全体ロードマップは追加済みです。運営モデル、指標定義、Decision Record、データ、分析成果物は未作成であり、実体が追加されるまではこの README からリンクしません。

## Issue 階層と開発の進め方

作業は次の階層で管理します。

- **Lv1:** Phase とその統合的な完了条件
- **Lv2:** Phase を構成する主要成果物・モデル
- **Lv3:** 設計・実装が可能な標準作業単位（原則 1 Pull Request）
- **Lv4:** 複数 PR、並行作業、個別の完了判定が必要な場合のみ設けるタスク

文書やモデルの変更は原則として Issue で目的と完了条件を示し、Pull Request で成果物の差分と判断理由をレビューします。現在の作業の起点は [Phase 0（Issue #1）](https://github.com/yuyuyu0706/data-value-scaling/issues/1) です。

階層の選択、Lv3 の分割パターン、Issue・Pull Request のライフサイクルは [Issue・Pull Request 管理ルール](docs/00_project/issue-pr-management.md) を参照してください。起票・作成時は [Issue テンプレート](.github/ISSUE_TEMPLATE/) と [Pull Request テンプレート](.github/pull_request_template.md) を入力補助として使用します。

## 関連リンク

- [Phase 0：プロジェクト管理環境を整備する（Issue #1）](https://github.com/yuyuyu0706/data-value-scaling/issues/1)
- [プロジェクト憲章と README を整備する（Issue #2）](https://github.com/yuyuyu0706/data-value-scaling/issues/2)
- [Repository README を整備する（Issue #5）](https://github.com/yuyuyu0706/data-value-scaling/issues/5)
- [プロジェクト憲章 Draft v0.1](docs/00_project/charter.md)
- [全体ロードマップ Draft v0.3](docs/00_project/roadmap.md)
- [文書管理ルール Draft v0.4](docs/00_project/document-governance.md)
- [Repository 構成ガイド Draft v0.4](docs/00_project/repository-structure.md)
- [Issue・Pull Request 管理ルール Draft v0.3](docs/00_project/issue-pr-management.md)
- [GitHub Project](https://github.com/users/yuyuyu0706/projects/6/views/1)
