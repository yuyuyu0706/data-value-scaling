# データ活用スケーリング計画 文書管理ルール

> **文書版:** Draft v0.2
>
> **位置付け:** 本文書は、プロジェクトの情報種別ごとの正本（Source of Truth）、更新方法、参照方向を定める正本です。文書の新設・変更時は本ルールを適用します。

## 1. 目的と適用範囲

本ルールは、同じ情報が複数の場所で独立して更新されることを避け、利用者が正しい参照先を判断できる状態を維持するためのものです。Repository 内の文書、GitHub Issue、Pull Request、GitHub Project の View と README に適用します。

運用では、情報ごとに正本を一つ決め、入口には要約と正本へのリンクだけを置きます。更新は定期実施ではなく、情報の意味・状態・参照先が変わるイベントを契機に行います。

## 2. 情報種別と正本

| 情報種別 | 正本 | 用途・正本に含める情報 | 主な更新責任 | 更新契機 | 主な参照元 |
| --- | --- | --- | --- | --- | --- |
| プロジェクトの背景・目的・主要概念・原則・対象範囲・成功状態 | [`charter.md`](charter.md) | 長期的で安定した判断基準 | 当該変更の Issue 担当者 | 目的、原則、スコープ、主要な定義または成功状態の合意変更 | Repository README、設計文書、Issue |
| プロジェクト概要と主要情報への入口 | [`README.md`](../../README.md) | 憲章の要約、主要モデルと Phase の概観、存在する成果物への導線 | 入口または成果物を変更する Issue 担当者 | 主要な参照先、全体像、現在 Phase の変更 | Repository トップ |
| 文書管理ルール | 本文書 | 正本、責務、更新・レビュー・参照・同期の共通ルール | 文書管理を変更する Issue 担当者 | 情報種別、正本、配置、参照または運用方法の変更 | Repository README、GitHub Project README、各成果物 |
| Repository の物理配置と領域の責務境界 | [`repository-structure.md`](repository-structure.md) | 現在の構成、配置判断、命名、構成変更基準 | Repository 構成を変更する Issue 担当者 | 領域、配置、命名または構成変更基準の変更 | Repository README、各領域 README、成果物追加 Issue |
| 各領域のローカルな利用案内 | [`docs/README.md`](../README.md)、[`decisions/README.md`](../../decisions/README.md)、[`definitions/README.md`](../../definitions/README.md)、[`data/README.md`](../../data/README.md)、[`analytics/README.md`](../../analytics/README.md) | 領域の目的、配置対象・対象外、利用開始時の確認先（上位ルールは再定義しない） | 当該領域を変更する Issue 担当者 | 領域の利用方法、主要な参照先または実装状態の変更 | Repository README、当該領域の利用者 |
| Phase・成果物・作業の目的、対象範囲、完了条件、依存関係、実施判断 | 対応する GitHub Issue | 実施前後の計画と完了判断 | Issue 担当者 | 起票、スコープ・依存関係・判断・完了状態の変更 | 親子 Issue、Project View、Pull Request |
| 現在の重点・ステータス・全体進捗 | [GitHub Project View](https://github.com/users/yuyuyu0706/projects/6/views/1) | Issue を横断した変動状態の表示 | Project 運営担当者または Issue 担当者 | Issue の着手、状態変更、優先対象の切替 | GitHub Project README、Repository README |
| 成果物の差分・レビュー・変更理由 | 対応する Pull Request | 正本を変更する差分とレビュー履歴 | Pull Request 作成者・レビュアー | 成果物の変更、レビュー指摘、マージ判断 | Issue、Git 履歴 |
| GitHub Project の利用案内 | [`github-project-readme.md`](github-project-readme.md) | Project の目的、見方、確認先 | Project 運営を変更する Issue 担当者 | 現在の重点、Project の見方または参照先の変更 | GitHub Project 本体の README |
| GitHub Project に表示する利用案内 | GitHub Project 本体の README | Repository 原稿の公開コピー（独自情報は持たない） | 原稿を変更する Pull Request の作成者または引継ぎ先 | Repository 原稿の変更がレビューされた後 | GitHub Project 利用者 |
| 永続的で複数成果物へ影響する設計判断 | Decision Record（整備後） | 判断、選択肢、理由、影響 | 判断を行う Issue 担当者 | 永続的な横断判断の合意 | Issue、設計文書、Pull Request |

5 領域の案内 README は追加済みですが、個別のロードマップ、運営モデル、指標定義、Decision Record、データ、分析成果物は未作成です。後続 Issue で目的、利用者、更新責任、既存の正本との境界を決め、実体が `main` に追加された後にこの表と入口文書へ追記します。

Decision Record の仕組みが整備されるまでは、永続的で複数成果物へ影響する判断を、関連 Issue の「重要な設計判断・論点」に理由と影響先を添えて記録します。将来の配置、テンプレート、採番方式を本 Draft では固定しません。

## 3. 各媒体の責務と参照方向

- **Repository README** は全体像を短く示す入口です。詳細な安定情報は憲章へ、現在の進捗は Project View と Issue へ、文書の扱いは本文書へ誘導します。
- **プロジェクト憲章** は長期的な判断基準の正本です。作業状況、詳細な実行順序、変更頻度の高い指標は管理しません。
- **GitHub Project README** は Project の利用方法と主要な確認先を案内します。安定情報や Issue ごとの詳細進捗を独立管理しません。
- **Project View** は現在状態を表示します。目的や完了条件を再記述せず、対応する Issue を参照します。
- **Issue** は実施単位の計画と完了判断を管理します。成果物本文や差分を複製せず、ファイルと Pull Request を参照します。
- **Pull Request** は差分、レビュー、変更理由を残します。固定的な説明の正本にはせず、マージ後の有効な内容は成果物から読めるようにします。

参照方向は、原則として **入口 → 正本、変動状態 → 計画、変更履歴 → 変更後の成果物** とします。正本側から入口の要約へ戻って内容を補完する構造にはしません。

## 4. 文書の追加・更新ルール

### 4.1 新しい成果物を追加する場合

1. Issue で成果物の目的、利用者、扱う情報、既存の正本との境界、更新責任と更新契機を定義します。
2. 既存の正本と重複する場合は新設せず、既存文書の更新または要約とリンクで解決できないか確認します。
3. 配置は [Repository 構成ガイド](repository-structure.md) に従います。構成ガイドで未確定のディレクトリを、本ルールだけで先行作成しません。
4. Pull Request で実体をレビューし、`main` へ追加された後に本文書の正本一覧と必要な入口へリンクを追加します。

### 4.2 重複と要約

- 同じ説明を複数箇所で独立管理しません。別の利用者向けに必要な場合は、正本の意味を変えない短い要約と正本へのリンクを掲載します。
- 要約には詳細な完了条件、数値、一覧など、正本と同時更新しなければ誤解を招く情報を極力含めません。
- 複製した情報が独自に更新され始めた場合、または同期確認が継続的に必要になった場合は、要約へ縮小して正本参照に切り替えます。
- 法令・ツール制約などにより複製が必要な場合は、正本、コピーである旨、同期責任と同期手順を明示します。GitHub Project README はこの例外に該当します。

### 4.3 リンク

- Repository 内は移動やブランチ上のレビューにも追従できる相対リンクを使用し、GitHub の Issue、Pull Request、Project など Repository 外の対象には完全な URL を使用します。
- 未作成文書を存在するようにリンクしません。「作成予定」と記し、実体が `main` に追加された後にリンクします。
- ファイルの改名・移動・削除時は、`rg` などで参照元を検索し、相対リンク、外部リンク、見出しアンカーを確認します。
- 外部リンクの変更を検知した場合は、代替の公式参照先へ更新するか、参照の必要性を見直します。

## 5. 更新・レビュー手順

変更を担当する Issue 担当者と Pull Request 作成者は、変更内容に応じて次を実施します。

1. 正本一覧から変更対象を特定し、正本を先に更新します。
2. 正本を要約・案内する入口文書、関連 Issue、Project View への影響を確認します。
3. 用語、Phase 名、Issue 階層、参照先を既存文書と照合します。
4. Pull Request に変更理由、影響する正本、確認方法、手動作業を記載します。
5. レビュアーは、正本の一意性、責務の重複、リンクの有効性、要約との整合、未作成文書へのリンクがないことを確認します。
6. マージまたは状態変更後に Project View を更新し、手動同期など Repository 外の残作業を Issue へ記録します。

背景・目的・原則・スコープを変える場合は憲章とその要約、Phase や主要成果物を変える場合は Repository README、Issue、Project View、現在の重点や Project の利用方法を変える場合は GitHub Project README 原稿と公開コピーを、それぞれ確認します。

## 6. GitHub Project README の手動同期

[`github-project-readme.md`](github-project-readme.md)を、Pull Request でレビューできる**正本**とします。GitHub Project 本体の README は、その内容を利用者へ表示するための**公開コピー**であり、Project 上だけで独自に編集しません。

同期は次の順序で行います。

1. Repository 原稿を変更し、Pull Request で内容とリンクをレビューします。
2. レビュー済みの原稿全体を GitHub Project 本体の README へ手動で反映します。
3. Project 本体を再表示し、見出し、表、箇条書き、リンク先が原稿と一致することを確認します。
4. 原稿と Project 表示を先頭から照合し、意図しない独自記述や反映漏れがないことを確認します。
5. 対応 Issue または Pull Request に、同期実施日、実施者、対象コミット、表示・リンク確認結果を記録します。

Repository 原稿の変更と Project 本体への反映を同時に完了できない場合は、対応 Issue の残アクティビティとして明示し、同期完了までは Issue を完了扱いにしません。Project 本体で緊急修正した場合も、同じ変更を直ちに Repository 原稿へ反映し、Pull Request の履歴を残します。

## 7. 変更時チェックリスト

- [ ] 変更する情報の正本を一意に特定した
- [ ] 正本以外は必要最小限の要約とリンクにした
- [ ] 更新責任とイベント駆動の更新契機を確認した
- [ ] 未作成文書へリンクしていない
- [ ] Repository 内の相対リンクと外部リンクが有効である
- [ ] 用語、Phase 名、Issue 階層、参照先が既存文書と整合している
- [ ] Markdown の見出し、表、箇条書き、末尾改行を確認した
- [ ] `git diff --check` を実行した
- [ ] GitHub Project README 原稿を変更した場合、公開コピーへ同期して記録した

CI や E2E が不要な文書のみの変更では、`git diff --check`、リンク先の存在確認、Markdown の目視確認を代替確認とし、その理由と結果を Pull Request に記録します。
