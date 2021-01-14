# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation  
## Users Table  
|Column|Type|Options|
|------|----|-------|
|name|string|null: false|
|email|string|null: false|
|password|string|null: false|  
<br>

### Association
- has_many :scores
- has_many :words  
<br>

## Scores Table  
|Column|Type|Options|
|------|----|-------|
|score|integer|null: false|
|user|references|null: false, foreign_key: true|  
<br>

### Association
- belongs_to :users  
<br>

## Words Table  
|Column|Type|Option|
|------|----|------|
|content|string|null: false|
|user|references|null: false, foreign_key: true|  
<br>

### Association  
- belongs_to :users
<br>
<br>

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
