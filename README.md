# README（共同開発要項）

## 目的
共同開発での開発フロー、コミュニケーションの取り方、ツールの使い方を体験すること

## 成果物
掲示板アプリ  
サンプル→ [転クエ掲示板](https://tenkue-board.herokuapp.com/)

## 参加要件
- 環境構築が完了し、指定バージョンに揃えられること（詳細は下記）
- ProgateでRuby、Railsを1周していること（もしくはそれと同程度のレベル感）
- GitHubアカウントを持っていること
- お互いを尊重して丁寧なコミュニケーションを取れること
- SlackやGitHubでのレスポンスをできる限り早く行えること（どんなに遅くても24時間以内）

## 人数とレビュー期間
- 1チーム3名
- メンターのレビュー期間は2週間

## 環境/技術
- Ruby 2.5.1
- Rails 5.2.4
- bundler 2.1.4
- PostgreSQL 12.2
- 記法：erb、Sass
- ソースコード管理：GitHub

## 機能要件
### [必須要件]
- ゲストユーザーログインができる
- 掲示板を投稿、編集、削除できる
- 掲示板に対してコメントが書き込める
- コメントの編集、削除ができる
- 掲示板に対していいねができる（いいねの取り消しもできる）
- 許可されていないページにアクセスするとrootパスへリダイレクト
- バリデーション、正規表現を適切に行う
- RSpecでモデルのテスト
- エラーメッセージを表示、日本語化
※詳細はTrello

## DB設計（ER図）
![ER図](https://user-images.githubusercontent.com/61058448/90863771-98856780-e3ca-11ea-8ec0-2a2b766ffec4.png)

# 共同開発を進める手順
1. 環境構築を完了していることを自ら確認
1. 指定バージョンに揃える
1. このリポジトリを下記手順にてクローン
    1. チームメンバー1人のGitHubでリポジトリ(A)を作成（リポジトリ名は任意）
    1. $ git clone https://github.com/Tenkue/tenkue_board.git
    1. $ git remote set-url origin リポジトリ(A)のURL
    1. $ git push origin master
1. [Trello](https://trello.com/b/ZEmfa89s/%E8%BB%A2%E3%82%AF%E3%82%A8%E5%85%B1%E5%90%8C%E9%96%8B%E7%99%BAissues%EF%BC%88%E3%83%86%E3%83%B3%E3%83%97%E3%83%AC%E3%83%BC%E3%83%88%EF%BC%89/user18257938/recommend)のテンプレートからボードを作成。載っている必須要件をそれぞれ実装
1. チーム内でコードレビューし、LGTM出たらメンターにコードレビュー依頼
1. メンターのLGTM出たらmasterブランチにマージ

## 注意点・特記事項
- クローンしたリポジトリは、チームメンバーいずれかのGitHubにプッシュすること（雛形のリポジトリに変更を加えないこと）
- 雛形のリポジトリには、devise周りの実装は完了してます
- ビューファイル、CSSファイルは用意したテンプレートファイルを利用してもOKです
- タグは自由に変更してもOKです（ただし必須要件の指示に従うこと）
- クラス名などは自由に変更してもOKです（ただしBEM記法は守ること）
- メンターのサポートはコードレビューのみです。技術的な質問は基本不可とさせてください（チーム内で調査＆解決を測ってください）
- メンターのレビュー対応期間は開発開始から2週間以内。それを超えたらレビューは行わない
- この共同開発の目的は、技術的なキャッチアップではなく「共同開発での開発フロー、コミュニケーションの取り方、ツールの使い方を体験すること」です。
