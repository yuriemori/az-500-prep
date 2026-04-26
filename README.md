# AZ-500 模擬試験 with GitHub Copilot
※元ネタ：https://github.com/runceel/lets-lean-mcp-architectの内容をAZ-500向けに変更<br>
Microsoft Azure Security Technologies（AZ-500）資格の取得を支援する学習ツールです。  
GitHub Copilot の **Skill** 機能を活用し、対話形式で模擬問題に取り組むことができます。

## 使い方

GitHub Copilot Chat（Copilot CLI や VS Code の Copilot Chat など）で、以下のように話しかけるだけで模擬試験が始まります。

```
問題を出して
```

```
クイズを出して
```

```
模擬試験を始めたい
```

Copilot が `az-500-quiz` スキルを自動的に実行し、AZ-500 の出題範囲に沿った模擬問題を出題します。

## 機能

- **シナリオベースの出題** — 架空の企業名・状況・要件を含む、実務に近い形式の問題
- **選択肢形式** — 4 つの選択肢（A〜D）から回答を選択
- **詳細なフィードバック** — 正解/不正解の表示に加え、各選択肢がなぜ正しい/不適切なのかを具体的に解説
- **分野のローテーション** — 偏りなく各分野から出題
- **連続出題** — 問題ごとに「次の問題に進む」か「終了する」かを選択可能。終了時には正答率のサマリーを表示

## 出題範囲

AZ-500 試験の出題範囲に準拠しています（2026年1月更新）。

| 分野 | 配点 |
|------|------|
| ID とアクセスのセキュリティ保護 | 15〜20% |
| ネットワークのセキュリティ保護 | 20〜25% |
| コンピューティング、ストレージ、データベースのセキュリティ保護 | 20〜25% |
| Microsoft Defender for Cloud と Microsoft Sentinel を使用した Azure のセキュリティ保護 | 30〜35% |

## 参考リンク

- [資格ページ](https://learn.microsoft.com/ja-jp/credentials/certifications/azure-security-engineer/)
- [試験ページ](https://learn.microsoft.com/ja-jp/credentials/certifications/exams/az-500/)
- [学習ガイド](https://learn.microsoft.com/ja-jp/credentials/certifications/resources/study-guides/az-500)
