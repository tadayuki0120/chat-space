## groups_usersテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|integer|null: false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|

<<<<<<< Updated upstream
### Association
- belongs_to :group
- belongs_to :user
=======
Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


## usersテーブル

|Column|Type|Options|
|------|----|-------|
|name|string|null: false|
|email|string|null: false|

### Association
-has_many :groups
-has_many :comments

## groupテーブル

|Column|Type|Option|
|------|----|------|
|name|string|null: false|
|user_id|integer|null: false, foreign_key: true|

### Association
-has_many :comment
blong_to :user

## commentsテーブル

|Column|Type|Option|
|------|----|------|
|text|text| |
|image|string| |
|group_id|integer|null :false, foreign_key: true|
|user_id|integer|null :false, foreign_key: true|

### Association
blong_to :user
blong_to :group
>>>>>>> Stashed changes
