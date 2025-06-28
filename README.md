# Bokrium

🌐 **サービスURL:** [https://bokrium.com](https://bokrium.com)

<table>
  <tr>
    <td width="65%">
      <img src="https://github.com/user-attachments/assets/9e836e20-4cea-44eb-bcbe-349ff85d751e" alt="左画像" width="100%">
    </td>
    <td width="30%">
      <img src="https://github.com/user-attachments/assets/51c9de56-0e39-4cb8-b490-816cd069af4d" alt="右画像" width="100%">
    </td>
  </tr>
</table>



| オートコンプリートで検索体験をスムーズに | 無限スクロールで快適な本棚体験 |
|------------------|---------------------|
| <p align="center"><img src="https://github.com/user-attachments/assets/fa07ebc9-84be-4a0d-8613-1318ae7e57be" width="250" alt="オートコンプリート"></p> | <p align="center"><img src="https://github.com/user-attachments/assets/c08fc27c-0d02-4553-b4db-b8fe40b75b3e" width="250" alt="無限スクロール"></p> |
| <p align="center">タイトルや著者名の一部を入力すると候補が表示。タイポや曖昧な記憶でも探しやすく。</p> | <p align="center">Turbo + Stimulus を用いた軽量な実装。表示冊数に応じてチャンク単位で読み込み</p> |




# 元書店員が開発した、知識を生活に活かす読書管理アプリ

本を「読むだけ」で終わらせず、  
知識を整理し、実践につなげるための読書管理アプリです。

## 🎯 こんな方におすすめ

- 本は好きだけど、読んだ内容を活かせていない  
- 同じ本をうっかり重複して買ってしまう  
- 自分の蔵書を整理して把握したい  
- 読書メモや気づきをあとで見返したい

## ✨ アプリの特徴

### 📚 バーコードスキャンで簡単登録  
ISBNを読み取るだけで、書籍情報を自分の本棚に追加できます。またキーワード検索にも対応しています。
| バーコードスキャン | キーワード検索 |
|------------------|---------------------|
| <p align="center"><img src="https://github.com/user-attachments/assets/f9d3e7f7-e6e6-49ed-81a5-be2186f1ae1c" width="250" alt="バーコードスキャン"></p> | <p align="center"><img src="https://github.com/user-attachments/assets/56efe725-fb4a-49a2-91d4-3e35a34cc117" width="250" alt="キーワード検索"></p> |
| <p align="center">ZXingを用いたクライアントサイドのバーコードスキャン機能。取得したISBNを非同期で送信し、複数のAPIから書誌情報を統合取得します。</p> | <p align="center">タイトル・著者をもとに、楽天・Google booksを切り替えて検索可能。ISBNでの検索も可能。</p> |

### 📝 読書メモ・画像を一元管理  
| [<img src="https://i.gyazo.com/aae1cfc3015d3347ce9ca9e7fa45c80c.gif" alt="本ごとのまとめ表示"  width="100%">](https://gyazo.com/aae1cfc3015d3347ce9ca9e7fa45c80c.gif) |  <img src="https://assets.bokrium.com/monkey.png" alt="monkey"> |
|---|---|

[![Image from Gyazo](https://i.gyazo.com/aae1cfc3015d3347ce9ca9e7fa45c80c.gif)](https://gyazo.com/aae1cfc3015d3347ce9ca9e7fa45c80c)

| ユーザー登録 / ログイン |
|-------------------------|
| [<img src="https://i.gyazo.com/33e39e655b45da69216e4b4b086500b8.gif" alt="本ごとのまとめ表示"  width="100%">](https://gyazo.com/33e39e655b45da69216e4b4b086500b8)|
| 『名前』『メールアドレス』『パスワード』『確認用パスワード』を入力してユーザー登録を行います。ユーザー登録後は、自動的にログイン処理が行われ、そのまま直ぐにサービスを利用できます。<br>また、Googleアカウントを用いてGoogleログインを行うことも可能です。 |

### 🔁 ランダム表示で学びを再発見  
過去の読書メモをランダムに表示。忘れかけていた知識を自然と思い出せます。

### 🔒 公開・非公開の切り替え  
メモは自分だけで管理することも、他のユーザーと共有することも可能です。

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
