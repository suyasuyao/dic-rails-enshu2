# 概要
Ruby on Rails入門シリーズ演習2【Blog機能を実装する】

# 機能
以下の要件を全て満たしていた場合のみ、合格とします。

- blog機能を作成すること
- blogの投稿・投稿確認・編集・一覧表示・削除機能があること
- blogの確認画面は、new -> createの時にのみ表示させ、edit -> updateの際には出現させないようにすること
- Githubにソースコードを送信し、そのリポジトリのURLを提出すること
- 1文字以上140文字以下しか投稿できないようにすること
- 140文字より多い文字数、または内容が空で投稿した場合、確認画面でエラーメッセージを表示させること

# docker
## 利用方法
```
# 初回のみ
 docker-compose build --no-cache
 docker-compose run web bin/rails db:create 
# マイグレーションやデータ投入を行う際に 
 docker-compose run web bin/rails db:migrate db:seed
# アプリケーション起動時毎回実施
 docker-compose up
```
