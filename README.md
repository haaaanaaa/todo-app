# テーブル設計

## users テーブル

| Column             | Type   | Options     |
| ------------------ | ------ | ----------- |
| name               | string | null: false |
| email              | string | null: false |
| encrypted_password | string | null: false |


-has many :tasks


## tasks テーブル

| column    |  Type  |  options    |
| --------- | ------ | ------------| 
| task_name | string | null: false | 
| task_due  | string | null: false | 

-belongs to :users



