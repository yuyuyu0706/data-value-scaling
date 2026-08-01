# データ活用スケーリング計画｜主要指標モデル構築

> **位置付け:** この README は GitHub Project を利用するための運営上の入口です。プロジェクト全体の説明や安定した定義は、[Repository README](https://github.com/yuyuyu0706/data-value-scaling#readme)と[プロジェクト憲章](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/charter.md)を参照してください。

## この Project の目的と利用対象

この Project は、データ活用スケーリング計画の Issue を整理し、現在の重点、作業の進行状況、次に確認・着手する対象を共有するために利用します。

主な利用対象は、プロジェクトの設計・運営担当者、各成果物の作成者・レビュアー、および進捗や判断経緯を確認する関係者です。

## 現在の重点

- **現在の Phase:** [Phase 0：プロジェクト管理環境を整備する（Issue #1）](https://github.com/yuyuyu0706/data-value-scaling/issues/1)
- **現在の主要成果物:** [全体ロードマップを策定する（Issue #29）](https://github.com/yuyuyu0706/data-value-scaling/issues/29)
- **現在の統合作業:** [ロードマップの参照導線と統合品質を整備する（Issue #32）](https://github.com/yuyuyu0706/data-value-scaling/issues/32)

詳細な進捗はこの README に複製せず、[Project の View](https://github.com/users/yuyuyu0706/projects/6/views/1)と各 Issue で確認します。

## View と作業の見方

1. [Project の View](https://github.com/users/yuyuyu0706/projects/6/views/1)で、Issue の状態と全体の進行状況を確認します。
2. 対象の Issue を開き、目的、対象範囲、完了条件、依存関係を確認します。
3. 実装や文書変更の差分とレビュー履歴は、Issue に関連付けられた Pull Request で確認します。
4. 次の作業は、現在の Phase と親 Issue の残アクティビティを起点に判断します。

Project に存在しない View や未作成の文書を前提にせず、現在のステータス・重点・全体進捗は Project View、目的・対象範囲・完了条件・依存関係は対応する Issue を正として確認してください。

## Issue 階層

- **Lv1:** Phase とその統合的な完了条件
- **Lv2:** Phase を構成する主要成果物・モデル
- **Lv3:** 設計・実装が可能な標準作業単位（原則 1 Pull Request）
- **Lv4:** 複数 PR、並行作業、個別の完了判定が必要な場合のみ設けるタスク

作業を確認するときは、まず Lv1 で現在の Phase、次に Lv2 で対象成果物を確認し、実際の設計・実装は Lv3（必要な場合のみ Lv4）からたどります。階層、分割、ライフサイクルの詳細は [Issue・Pull Request 管理ルール](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/issue-pr-management.md) を参照してください。

## 正式文書と管理情報

| 確認したい情報 | 参照先 |
| --- | --- |
| プロジェクト概要、主要 KPI・モデル、Phase の短い要約 | [Repository README](https://github.com/yuyuyu0706/data-value-scaling#readme) |
| 背景、定義、基本原則、対象範囲、成功状態 | [プロジェクト憲章 Draft v0.1](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/charter.md) |
| Phase 0〜6の実行順序、成果ゲート、依存関係、引継ぎ | [全体ロードマップ Draft v0.2](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/roadmap.md) |
| 情報種別ごとの正本、更新責任、参照・同期ルール | [文書管理ルール Draft v0.4](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/document-governance.md) |
| Issue 階層、ライフサイクル、関連付け、状態管理 | [Issue・Pull Request 管理ルール Draft v0.2](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/issue-pr-management.md) |
| Phase、成果物、作業単位、完了条件 | [Issues](https://github.com/yuyuyu0706/data-value-scaling/issues) |
| 現在の重点と進捗 | [GitHub Project](https://github.com/users/yuyuyu0706/projects/6/views/1) |
| 変更差分、レビュー、変更理由の履歴 | [Pull requests](https://github.com/yuyuyu0706/data-value-scaling/pulls) |

## 更新と Repository 原稿との同期

この README では、現在の Phase、主要作業、確認先だけを更新対象とし、プロジェクトの安定情報や詳細な進捗は複製しません。

Repository の [`docs/00_project/github-project-readme.md`](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/github-project-readme.md)をレビュー可能な正本とし、GitHub Project 本体の README は公開コピーとして扱います。原稿の変更を Pull Request でレビューした後、Project 本体へ手動反映し、表示内容とリンクの一致を確認して、対応 Issue または Pull Request に同期結果を記録します。詳細な手順は[文書管理ルール](https://github.com/yuyuyu0706/data-value-scaling/blob/main/docs/00_project/document-governance.md#6-github-project-readme-の手動同期)を参照してください。
