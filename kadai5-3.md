## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
* エンドポイント:https://api.zipaddress.net
* 機能日本の郵便番号を基に住所情報を取得する。郵便番号を入力すると、それに関連する住所（都道府県、市区町村、町名など）を返す。
* リクエストとレスポンスのフォーマット
* リクエストフォーマット:HTTPメソッド: GET
URL例: https://api.zipaddress.net/?zipcode=1000001
クエリパラメータ: zipcode
  レスポンスフォーマット
  JSON形式
{
  "code": 200,
  "data": {
    "fullAddress": "東京都千代田区千代田",
    "pref": "東京都",
    "city": "千代田区",
    "town": "千代田"
  }
}
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
* API名称:JSONPlaceholder
* 参照URL: JSONPlaceholder
* エンドポイントと機能
* エンドポイント: /posts/{id}
機能: サンプルの投稿データを取得する。投稿IDを指定すると、その投稿のタイトルや内容を取得できる。
* リクエストとレスポンスのフォーマット
* リクエストフォーマット:HTTPメソッド: GET
URL例: https://jsonplaceholder.typicode.com/posts/1
レスポンスフォーマット:JSON形式
{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
  "body": "quia et suscipit\nsuscipit..."
}
### Q3-3. 感想
* 今回の課題で苦労したこと
* 適切なAPIを見つけるのに時間がかかった。特に、リクエストとレスポンスのフォーマットを正確に理解することが難しかった。
* 演習を通して理解できたこと
* APIのリクエストとレスポンスの構造を理解し、どのようにデータがやり取りされるのかを学んだ。
* Web APIの利便性や課題など
* 利便性:Web APIを使用することで、他のサービスと簡単に連携できるため、アプリケーションの機能を拡張するのが容易になる。例えば、リアルタイムのデータを取得したり、外部サービスの機能を利用したりできる。
* 課題: APIの信頼性やレスポンス時間、エラーハンドリングの難しさなどが課題である。また、APIの変更や廃止によって、依存しているアプリケーションが影響を受ける可能性もある。
