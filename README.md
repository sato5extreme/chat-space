DB設計
## ユーザー登録

|Column|Type|Options|
|------|----|-------|
|id|BIGINT|auto in|
|name|VARCHAR|null: false, foreign_key: true|
|e-mail|VARCHAR|null: false, foreign_key: true|
|password|VARCHAR|null: false|

### Association
- belongs_to :group
- belongs_to :user


## 投稿機能
|Column|Type|Options|
|------|----|-------|
|text|text|null: false|
|image|TEXT||
|create_at|DATETIME||
|update_at|DATETIME||

### Association
- belongs_to :group
- belongs_to :user

## グループ管理
|Column|Type|Options|
|------|----|-------|
|

### Association
- belongs_to :tweets
- belongs_to :user