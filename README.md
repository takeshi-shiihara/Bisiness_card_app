# README

## usersテーブル
|Column|Type|Options|
|------|----|-------|
|name|string|null:false|
|password|string|null:false|


## cardsテーブル
|Column|Type|Options|
|------|----|-------|
|campany|string|null:false|
|position_id|references|foreign_key:true|
|name|string|null:false|
|phone_number|integer|null:false|
|e-mail|string|null:false|

### Association
has_many:images
belongs_to:position


## imagesテーブル
|Column|Type|Options|
|------|----|-------|
|card_id|references|null:false|

### Association
belongs_to:card


## positionsテーブル
|Column|Type|Options|
|------|----|-------|
|position|string||
|ancestry|string|index:true|

### Association
has_many:card
has_ancestry




This README would normally document whatever steps are necessary to get the
application up and running.

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
