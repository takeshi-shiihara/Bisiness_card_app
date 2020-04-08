# README

##cardsテーブル
|Column|Type|Options|
|------|----|-------|
|campany|string||
|position_id|references|foreign_key:true|
|name|string|

#Association
has_many:images


##imagesテーブル
|Column|Type|Options|
|------|----|-------|
|card_id|reference|null:false|

#Association
belongs_to:card

##usersテーブル
|Column|Type|Options|
|------|----|-------|
|name|string|null:false|
|







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
