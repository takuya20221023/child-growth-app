# 👶 こどもメモリー（仮）　*画像は順次実装予定です。

## アプリケーション概要

**こどもメモリー（仮）** は、子どもの成長記録を「写真・動画・コメント」で残し、家族と共有できるアプリケーションです。  
月齢別のチェックリスト機能や、タイムライン・カレンダーでの表示機能を備え、大切な思い出を時系列で簡単に振り返ることができます。

---

## URL

※デプロイ完了後に追記予定

---

## テスト用アカウント

- メールアドレス：`test@example.com`  
- パスワード：`password123`  
- Basic認証：admin 2222

---

## 利用方法

1. ユーザー登録・ログイン
2. 子どものプロフィールを登録
3. 成長記録（写真・動画・コメント）を投稿
4. タイムラインまたはカレンダーで記録を確認
5. 月齢チェックリストで成長の確認と記録

---

## アプリケーションを作成した背景

子育て中に以下のような課題を感じていました。

- 成長記録がスマホの中で埋もれてしまう
- SNSではプライバシー面で不安がある
- 家族全員で思い出を簡単に共有したい
- 月齢ごとの成長チェックを記録していきたい

このような背景から、「成長を大切に残し、安心して家族と共有できる」アプリを目指して制作しました。

---

## 実装した機能と画面イメージ

### ホーム画面（ダッシュボード）

- 成長記録がタイムライン形式で表示されるトップページです。

![home](app/assets/images/readme/home.png)

---

### 成長記録投稿画面

- 写真・動画・コメント付きで記録を残せます。

![new_record](app/assets/images/readme/new_record.png)

---

### カレンダー表示

- 日ごとの記録をカレンダー形式で確認可能です。

![calendar](app/assets/images/readme/calendar.png)

---

### 月齢チェックリスト

- 子どもの発達チェックを月齢に応じて管理できます。

![checklist](app/assets/images/readme/checklist.png)

---

## 実装予定の機能

- 音声記録機能（ボイスで思い出を保存）
- フォトブック生成機能（記録から冊子化）
- 家族招待機能（メールやQRコードで簡単共有）

---

## データベース設計（ER図）

![ER図](app/assets/images/readme/er_diagram.png)

---

## 画面遷移図

![画面遷移図](app/assets/images/readme/screen_flow.png)

---

## 開発環境

- フレームワーク：Ruby on Rails 7
- 言語：HTML / CSS / JavaScript
- CSS：Tailwind CSS（予定）またはBootstrap
- 認証機能：Devise
- DB：MySQL
- ファイルアップロード：Active Storage
- カレンダー表示：simple_calendar / FullCalendar
- デプロイ：Render

---

## ローカルでの動作方法

以下の手順でローカル環境にセットアップできます。

git clone https://github.com/your-username/kodomo-memory.git
cd kodomo-memory
bundle install
rails db:create
rails db:migrate
rails s

## 工夫したポイント
おじいちゃん・おばあちゃんにも使いやすいシンプル設計

カレンダー表示やチェックリストによる多角的な成長記録

Deviseでセキュアな認証、Active Storageでメディア管理

モバイルファーストのUI設計を意識

## 改善点
投稿編集・削除機能のUI強化

通知機能の追加（コメント追加など）

複数家族との共有に対応するアーキテクチャ検討

## 制作時間
約〇〇時間（随時更新）

```bash