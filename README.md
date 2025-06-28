# Bokrium

🌐 **サービスURL:** [https://bokrium.com](https://bokrium.com)

[![Image from Gyazo](https://i.gyazo.com/339ded291d706d0b69c11956dbf3732c.png)](https://gyazo.com/339ded291d706d0b69c11956dbf3732c)

# 元書店員が開発した読書管理アプリ

本を「読むだけ」で終わらせず、  
知識を整理し、実践につなげるための読書管理アプリです。

## 🎯 こんな方におすすめ

- 本は好きだけど、読んだ内容を活かせていない  
- 同じ本をうっかり重複して買ってしまう  
- 自分の蔵書を整理して把握したい  
- 読書メモや気づきをあとで見返したい

## ✨ アプリ機能紹介

<br><h3 align="center">📧 ユーザー登録</h3>

|  メールログイン | LINEログイン |
|:--:|:--:|
| [<img src="https://i.gyazo.com/5e18a488462bc89b0cd65dee2d628bcd.png" alt="アカウント登録画面" width="100%">](https://gyazo.com/5e18a488462bc89b0cd65dee2d628bcd) | [<img src="https://i.gyazo.com/e35992b842ae24c8149e96275682ff9b.png" alt="LINEログイン画面" width="95%">](https://gyazo.com/e35992b842ae24c8149e96275682ff9b) |

アカウント登録にはDeviseによるメール認証を採用しており、安全性を確保しつつ、確認メールのリンクをクリックするだけで自動的にログインできます。登録後のパスワード再設定も、メール送信によるリンク経由で安心して実施可能です。また、LINEログインにも対応しており、メールアドレスやパスワードの入力なしで、ワンタップで簡単に登録・ログインができます。

<br><h3 align="center">🤳📚 書籍登録</h3>

| バーコードスキャン | キーワード検索 |
|------------------|---------------------|
| <p align="center"><a href="https://gyazo.com/88615713f29c4da2bd917487a84d9f53"><img src="https://i.gyazo.com/88615713f29c4da2bd917487a84d9f53.gif" width="250" alt="バーコードスキャンGIF"></a></p> | <p align="center"><img src="https://github.com/user-attachments/assets/56efe725-fb4a-49a2-91d4-3e35a34cc117" width="250" alt="キーワード検索"></p> |
| <p align="center">ZXingを用いたクライアントサイドのバーコードスキャン機能。取得したISBNを非同期で送信し、複数のAPIから書誌情報を統合取得します。</p> | <p align="center">タイトル・著者をもとに、楽天・Google Booksを切り替えて検索可能。ISBNでの検索も可能。</p> |

<br><h3 align="center">📚👀 本棚</h3>

| ビューと表示冊数を選べる本棚 |
|-------------------------|
| <p align="center">[<img src="https://i.gyazo.com/fb85667d739a8c62f3abab2a9703d247.png" alt="本棚一覧画像" width="100%">](https://gyazo.com/fb85667d739a8c62f3abab2a9703d247)</p> |
| <p align="center">[<img src="https://i.gyazo.com/7a994cfc549125f3977c8f87e03daae5.png" alt="棚設定UI" width="100%">](https://gyazo.com/7a994cfc549125f3977c8f87e03daae5)</p> |
| <p align="center">[<img src="https://i.gyazo.com/262949cb147fe5434171f211b7c5864d.gif" alt="本棚レイアウト切り替えGIF" width="100%">](https://gyazo.com/262949cb147fe5434171f211b7c5864d)</p> |
| 書籍ごとに読書メモ・タグ・画像をまとめて保存。5つの本棚レイアウトを自由に切り替えて、見やすく振り返りやすい読書体験を提供します。 |

<br><h3 align="center">📝 メモ機能</h3>

| 📝 本ごとにメモ・画像・タグをまとめて管理 |
|-------------------------|
| <p align="center">[<img src="https://i.gyazo.com/33e39e655b45da69216e4b4b086500b8.gif" alt="本ごとのまとめ表示" width="100%">](https://gyazo.com/33e39e655b45da69216e4b4b086500b8)</p> |
| 読書メモには、Markdown対応のTipTapエディタを採用。見出しや箇条書きなどを使いながら、自由にリッチな記録ができます。画像はS3に保存され、スムーズに管理可能です。<br><br>さらに、タグ付けや書籍情報の編集、読書中・読みたい・読了といったステータスの設定にも対応。<br><br>通常表示では、左上に拡大・縮小ボタン、右上に「非公開・リンク限定・公開」から選べる公開設定メニューが表示されます。モーダル表示では、メモの文字数や作成日・更新日も確認できます。 |

| 💌 ランダムメモをLINE・メールで通知 |
|-------------------------|
| <p align="center">[<img src="https://i.gyazo.com/824716aad7a7d4a02f4e184eb7c3ee63.png" alt="メモ通知UIイメージ" width="100%">](https://gyazo.com/824716aad7a7d4a02f4e184eb7c3ee63)</p> |
| 登録済みの読書メモの中から、毎朝ランダムに1件を選んでLINEまたはメールでお届けします。<br>「あの本、こんなこと書いてたな」と自然に思い出せる、ちょっと嬉しい仕組みです。 |


### 🔒 公開・非公開の切り替え  
メモは自分だけで管理することも、他のユーザーと共有することも可能です。



| オートコンプリートで検索体験をスムーズに | 無限スクロールで快適な本棚体験 |
|------------------|---------------------|
| <p align="center"><a href="https://gyazo.com/087b7bf154e1baab02d44c3a45e787be"><img src="https://i.gyazo.com/087b7bf154e1baab02d44c3a45e787be.gif" width="250" alt="オートコンプリートGIF"></a></p> | <p align="center"><img src="https://github.com/user-attachments/assets/c08fc27c-0d02-4553-b4db-b8fe40b75b3e" width="250" alt="無限スクロール"></p> |
| <p align="center">タイトルや著者名の一部を入力すると候補が表示。タイポや曖昧な記憶でも探しやすく。</p> | <p align="center">Turbo + Stimulus を用いた軽量な実装。表示冊数に応じてチャンク単位で読み込み</p> |

## 🛠 開発の背景

私は書店に約5年間勤めていました。  
本好きなお客様と接する中で、「読んでもなかなか活かせない」と感じる声を多く聞いてきました。

私自身も、蔵書が増えていくなかで同じ本を重複して買ってしまったことがあります。  
また、読んだ内容をきちんと整理し、日々に活かすためには「ただ読むだけ」では不十分だと感じるようになりました。

そこで、  
**蔵書の管理、知識の整理、そして日常への活用までをサポートするアプリ**を、自分自身の欲しかった形で作ることにしました。

## 📦 できることまとめ

- 書籍をバーコードから一発登録  
- メモ・タグ・画像を自由に追加  
- メモをランダムに表示して知識を再発見  
- メモの公開・非公開を切り替え可能  
- 他のユーザーと読書メモを共有・発見


## 🛠 使用技術

| カテゴリ       | 技術構成                                                                                                      |
|----------------|---------------------------------------------------------------------------------------------------------------|
| フロントエンド | Stimulus / Turbo / React（TipTap専用） / ESBuild / JavaScript                                                |
| バックエンド   | Ruby 3.4.3 / Ruby on Rails 8.0.2                                                                              |
| データベース   | PostgreSQL（Neon） / pg_search                                                                               |
| 認証           | Devise（メール・LINEログイン対応)                    |
| 環境構築       | Docker / dotenv-rails / fly.toml / Procfile.dev                                                              |
| CI/CD          | GitHub ActionsでPR時にRuboCop・Brakeman・RSpecを実行、mainマージ時にFly.ioへ自動デプロイ。                        |
| インフラ       | Fly.io、Amazon S3 + CloudFront（画像配信）、Namecheap（独自ドメイン）         |
| 画像処理       | Active Storage / Amazon S3 / CDN署名付きURL配信                                                              |
| メモエディタ   | TipTap（Reactベース WYSIWYGエディタ）                                                                        |
| 通知機能       | LINE Messaging API（定期メモ通知）、ActionMailer（メール通知）                                   |
| 支援機能       | Stripe（寄付・マンスリーサポート）                                                                           |
| 検索・UX       | 無限スクロール（Turbo + Stimulus）、オートコンプリート（書籍タイトル・著者）、フィルター・ソート機能          |
| その他         | Bootstrap / Kaminari / Pagy /                                     |



# ER図

<img src="https://assets.bokrium.com/bokrium_erd.png" alt="ER図" width="100%" />
