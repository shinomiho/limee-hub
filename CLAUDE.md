# リミー コントロールセンター — Claude Code 文脈ファイル

このファイルを読んだClaudeは、リミーのシステム全体を把握した状態で作業を開始できます。

---

## ⚠️ プロジェクト境界（最重要・2026-06-03追加）

### このディレクトリで扱う対象
**limee-hub（コントロールセンター）の編集のみ**

ここはリミー全体の情報を一覧する場所であって、**各事業の中身を直接編集する場所ではない**。
- 例外：HTML/CSS のリンクや表示の調整は OK
- NG：「limee-hub から AI診断のguide.htmlを直接いじる」など、別ディレクトリのファイルに手を出す

### 他事業のファイルを編集したくなったら
1. 「これは別プロジェクトの作業ですね」と認識を示す
2. メモリ `cross_project_concerns.md` への追加を提案
3. 「次に該当プロジェクトのセッションで対応しましょう」と延期

### 「ついで修正」は禁止
limee-hub のリンク追加で気づいた他事業の改善ポイントは、その場で着手しない。
気になりリストに残して、別セッションで該当プロジェクトに移動して扱う。

---

## リミーとは

- **サービス名**：リミー（Rimee）
- **代表**：Miho Shinohe（四戸美穂）miho.shinohe@gmail.com / miho.shinohe@remenow.com
- **事業内容**：入社後90日に特化した採用後支援HRテック。AI診断・人的資本KPI設計・ESG経営支援コンサルティング
- **主要ターゲット**：上場企業・IPO準備企業・ESG経営に取り組む中堅〜大手企業（to B）

---

## GitHubアカウント・リポジトリ一覧

- **GitHubアカウント**：shinomiho
- **limee-hub**（このリポジトリ）：https://github.com/shinomiho/limee-hub
  - コントロールセンター（引き継ぎ・運用ダッシュボード）
  - 公開URL：https://shinomiho.github.io/limee-hub/
- **remenow-site**：https://github.com/shinomiho/remenow-site
  - 公式Webサイト（remenow.tokyo）
  - 公開URL：https://remenow.tokyo/
  - ローカルパス：/Users/mihomatuo/Downloads/remenow-site/
- **onboarding-diagnosis**：https://github.com/shinomiho/onboarding-diagnosis
  - AI診断システム（入社90日）
  - 公開URL：https://shinomiho.github.io/onboarding-diagnosis/

---

## remenow.tokyo 公式サイト

| 項目 | 内容 |
|------|------|
| ページ構成 | index.html / service.html / company.html / faq.html / representative.html / contact.html / privacy.html / tokushoho.html |
| Google Analytics 4 | 測定ID: G-EQ9HFMXHJV（2026-05-15設置） |
| GA4管理URL | https://analytics.google.com/analytics/web/#/a374442210p512366786/reports/ |
| メール登録ポップアップGAS URL | https://script.google.com/macros/s/AKfycbx8mMDTyAvhC9tdE1t7XYA2kWTvCYQTcqU02bLOnfwutg0OXOdgye4S6OlyI_smRg1q/exec |
| メール登録データ保存先 | https://docs.google.com/spreadsheets/d/1b06wFoZvyUr4kaXJURAN7Qe5r6iTRQRYPuOnlQuJz8U/edit （「メール登録」シート） |
| 個別相談予約（Spir） | https://app.spirinc.com/t/BaVcJLzp1EBNlPmMopnQj/as/nEkvuC6zy3wU2bD10nCV0/confirm |

---

## AI診断システム（onboarding-diagnosis）

| 項目 | 内容 |
|------|------|
| GAS URL | https://script.google.com/macros/s/AKfycbyGceshWFX-_kepVh5KHTvNwsrNAh7hW22U48KSp4DVvohXurOsAa6BDW7MFrsbKJ0n/exec |
| 企業登録URL | https://shinomiho.github.io/onboarding-diagnosis/register.html?token=REME2026 |
| 管理画面 | https://shinomiho.github.io/onboarding-diagnosis/admin.html |
| 従業員管理画面 | https://shinomiho.github.io/onboarding-diagnosis/company-admin.html?code=LIMEE_XXXXXX |
| 導入ガイド | https://shinomiho.github.io/onboarding-diagnosis/guide.html |
| 使用AI | Claude claude-sonnet-4-6（Anthropic API） |
| データ保存 | Googleスプレッドシート（responses / companies / monthly_reports / manager_actions / employees） |

### 機能概要
- 25問診断 → AIレポート生成 → 本人・マネージャーへメール自動送信
- 企業自己登録 → 専用URLを自動発行 → ウェルカムメール自動送信
- 月次レポート自動配信（毎月1日・15日）
- アクションチェックリマインド（毎月5日・20日）
- KPIダッシュボード（管理画面内）

---

## SNS自動投稿システム

| 項目 | 内容 |
|------|------|
| ローカルパス | /Users/mihomatuo/social-auto-post/apps-script.gs |
| GASプロジェクト | https://script.google.com/home/projects/1kWqpYwUyRRNdjGO9-cHrloLhgwCuNR-5-ph2hyHCKc4T4iv1eAbgoZV6/edit |
| 実行タイミング | 毎朝8時（GASトリガー自動実行） |
| 対象SNS | LinkedIn / Instagram / LINE公式 |
| CTAファネル | STEP1（離職リスク診断）→ STEP2（個別無料相談） |
| STEP1 URL | https://shinomiho.github.io/-reme-risk-diagnosis/ |
| STEP2 URL | https://app.spirinc.com/t/BaVcJLzp1EBNlPmMopnQj/as/nEkvuC6zy3wU2bD10nCV0/confirm |

---

## SNSアカウント

- LinkedIn: https://www.linkedin.com/in/miho-shinohe/
- Instagram: https://www.instagram.com/shinomiho_reme_hrtech/
- LINE公式アカウント：LINE Official Account Managerで管理

---

## 重要アカウント情報

| サービス | アカウント |
|---------|----------|
| Googleアカウント（メイン） | miho.shinohe@remenow.com |
| Googleアカウント（個人） | miho.shinohe@gmail.com |
| GitHubアカウント | shinomiho |
| ※パスワード・APIキー | パスワードマネージャーまたはMihoから口頭で入手 |

---

## 契約書管理システム（2026-05-18〜稼働）

| 項目 | 内容 |
|------|------|
| 電子署名 | GMOサイン（無料プラン・月5件）https://www.gmo-sign.com/ |
| Driveフォルダ | 📋 契約書管理 / ✅ 締結済 / 🔄 交渉中 / 📁 期限切れ・アーカイブ |
| 契約書台帳 | https://docs.google.com/spreadsheets/d/1z8t4o2EemRvrB7GZGC44TXD9o8FyKq5pmXK4hhWbRM8 |
| GASプロジェクト名 | 契約書管理 |
| 締結済フォルダID | 1y-ETnWPUxffBeeDX9FotXufQ4FztElhA |

### GAS関数・トリガー
- `syncNewContracts`：1時間おき → 締結済フォルダの新規ファイルを台帳に自動登録
- `checkDeadlines`：毎日午前9時 → 終了日60日以内の契約をメール通知（30日以内は【要対応】）

### 運用手順
1. GMOサインで締結 → PDFダウンロード → Drive「✅ 締結済」に保存
2. 1時間以内に台帳へ自動登録される
3. 台帳で取引先名・契約種別・**終了日**・自動更新を手入力（終了日必須）

---

## 運用ルール・注意事項

- Webサイトを修正したら `git add → git commit → git push` でGitHub Pagesに反映
- スプレッドシートの列を削除・移動しない（GASが列の位置を参照している）
- GASのトリガーを無断で追加・削除しない（二重送信・停止の原因になる）
- コード変更後はGASを「新バージョンとしてデプロイ」する（保存だけでは反映されない）

---

## このコントロールセンターの目的

Mihoが不在でも**誰でも運用できる**状態を作ること。
このCLAUDE.mdを読んだClaudeはリミーの全文脈を持ってすぐに作業できます。
「〇〇を変更したい」「〇〇が壊れた」など日本語で話しかけてください。
