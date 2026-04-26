---
name: az-500-quiz
description: >-
  AZ-500（Microsoft Azure Security Technologies）の模擬問題を出題するスキル。
  ユーザーが「問題を出して」「クイズ」「模擬試験」「練習問題」などと言ったときに使用する。
---

## 概要

AZ-500 試験の模擬問題を出題し、ユーザーの回答に対してフィードバックを行う。

## 出題範囲

以下の 4 分野から出題する。配点の高い分野を優先的に出題すること。

| 分野 | 配点 |
|------|------|
| ID とアクセスのセキュリティ保護 | 15〜20% |
| ネットワークのセキュリティ保護 | 20〜25% |
| コンピューティング、ストレージ、データベースのセキュリティ保護 | 20〜25% |
| Microsoft Defender for Cloud と Microsoft Sentinel を使用した Azure のセキュリティ保護 | 30〜35% |

## Microsoft Learn からの情報取得

問題や解説の精度を高めるために、`microsoftlearn-microsoft_docs_search` ツールや `microsoftlearn-microsoft_docs_fetch` ツールを活用して Microsoft Learn の公式ドキュメントから情報を取得できる。

### 活用シーン

- 最新のサービス仕様や制約を確認してから問題を作りたいとき
- サービス比較（例: NSG vs Azure Firewall、Microsoft Defender for Cloud vs Microsoft Sentinel）の正確な違いを調べたいとき
- フィードバックに公式ドキュメントの URL を含めてユーザーの学習を支援したいとき

### 検索クエリの例

- `"Microsoft Entra ID Conditional Access"` — 条件付きアクセス設計
- `"Azure NSG vs Azure Firewall"` — ネットワークセキュリティ比較
- `"Microsoft Defender for Cloud recommendations"` — クラウドセキュリティ態勢管理
- `"Microsoft Sentinel analytics rules"` — SIEM / SOAR 設計
- `"Azure Key Vault access policies RBAC"` — キーとシークレット管理
- `"Azure Storage encryption customer-managed keys"` — ストレージ暗号化

## 出題手順

1. 問題を 1 問ずつ出題する
2. 問題文にはシナリオ（架空の企業名・状況・要件）を含め、実務に近い形式にする
3. 選択肢は 4 つ（A〜D）用意する
4. 選択肢の提示には必ず `ask_user` ツールを使い、ユーザーが選択肢を選べるようにする
5. `ask_user` の `allow_freeform` は `false` に設定する

## 回答後のフィードバック

ユーザーの回答後、以下の構成でフィードバックを提供する：

1. **正解/不正解の表示**
2. **正解の選択肢が正しい理由** — Azure 公式ドキュメントに基づいた具体的な説明
3. **不正解の選択肢がなぜ不適切か** — 表形式で各選択肢の問題点を簡潔に示す
4. **試験のポイント** — この問題から学ぶべき重要な考え方やキーワードの整理

## フィードバック後の進行

フィードバック提供後、`ask_user` ツールで「次の問題に進む」か「終了する」かを確認する。
終了時は正答数/出題数のサマリーを表示する。

## 出題のガイドライン

- 同じ分野の問題が連続しないよう、分野をローテーションする
- 難易度は実際の AZ-500 試験に合わせる
- 選択肢には「もっともらしいが不正解」な選択肢を含め、理解度を測れるようにする
- Azure のセキュリティサービス比較（例: NSG vs Azure Firewall、Microsoft Defender for Cloud vs Microsoft Sentinel、Azure AD B2C vs Microsoft Entra External ID）を問う問題を適宜含める
- すべて日本語で出題・解説する

## 参考リンク

- 資格ページ: https://learn.microsoft.com/ja-jp/credentials/certifications/azure-security-engineer/
- 試験ページ: https://learn.microsoft.com/ja-jp/credentials/certifications/exams/az-500/
- 学習ガイド: https://learn.microsoft.com/ja-jp/credentials/certifications/resources/study-guides/az-500
