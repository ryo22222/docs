# GET /v1/me

自分のプロフィール情報を取得することができます。

## フィールド

| 名前 | 概要 |
| --- | --- |
| id | ユーザID |
| username | URLなどで使用されているユーザ名 |
| name | ユーザの名前 |
| description | プロフィール |
| url | ユーザのURL |
| avatar_url | アバター画像 |
| background_image_url | 背景画像 |
| records_count | 記録数 |
| followings_count | ユーザがフォローしている人の数 |
| followers_count | ユーザをフォローしている人の数 |
| wanna_watch_count | ステータスを「見たい」にしている作品の数 |
| watching_count | ステータスを「見てる」にしている作品の数 |
| watched_count | ステータスを「見た」にしている作品の数 |
| on_hold_count | ステータスを「中断」にしている作品の数 |
| stop_watching_count | ステータスを「中止」にしている作品の数 |
| created_at | ユーザ登録した日時 |
| email | ユーザのメールアドレス |
| notifications_count | 通知数 |


## パラメータ

| 名前 | 概要 | 使用例 |
| --- | --- | --- |
| fields | レスポンスボディに含まれるデータのフィールドを絞り込みます。 | fields=id,username |


## リクエスト例

```
$ curl -X GET https://api.annict.com/v1/me?access_token=(access_token)
```

```json
{
  "id": 2,
  "username": "shimbaco",
  "name": "Koji Shimba",
  "description": "アニメ好きが高じてこのサービスを作りました。聖地巡礼を年に数回しています。",
  "url": "http://shimba.co",
  "avatar_url": "https://api-assets.annict.com/paperclip/profiles/1/tombo_avatars/master/d8af7adc8122c96ba7639218fd8b5ede332d42f2.jpg?1431357292",
  "background_image_url": "https://api-assets.annict.com/paperclip/profiles/1/tombo_background_images/master/ee15d577fb2f2d61bdaf700cfab894b286a5762d.jpg?1486753229",
  "records_count": 2369,
  "followings_count": 258,
  "followers_count": 205,
  "wanna_watch_count": 237,
  "watching_count": 103,
  "watched_count": 335,
  "on_hold_count": 45,
  "stop_watching_count": 244,
  "created_at": "2014-03-02T15:38:40.000Z",
  "email": "me@shimba.co",
  "notifications_count": 0
}
```
