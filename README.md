
## usersテーブル
|Column|Type|Options|
|------|----|-------|
|name|string|null: false|
|email|string|null: false|
### Association
- has_many :groups
- has_many :comments

## groupテーブル
|Column|Type|Option|
|------|----|------|
|name|string|null: false|
|user_id|integer|null: false, foreign_key: true|
### Association
- has_many :comment
- blong_to :user


## commentsテーブル
|Column|Type|Option|
|------|----|------|
|text|text| |
|image|string| |
|group_id|integer|null :false, foreign_key: true|
|user_id|integer|null :false, foreign_key: true|
### Association
- blong_to :user
- blong_to :group


