# README

# テーブル設計
## usersテーブル
| Column             |  Type   | Option       |key
| ------------------ | ------- | ------------ |
| email              | string  | null :false  |UNI
| encrypted_password | string  | null :false  |
| name               | string  | null :false  |
| profile            | text    | null :false  |
| occupation         | text    | null :false  |
| position           | text    | null :false  |
## commentsテーブル
| Column    | Type    | Options     |key
| --------- | ------- | ----------- |
| content   | text    | null: false |
| prototype |reference| null :false |foreign_key
| user      |reference| null :false |foreign_key
## prototypesテーブル
| Column    | Type    | Options     |key
| --------- | ------- | ----------- |
| title     | string  | null: false |
|catch_copy | text    | null :false |
| concept   | text    | null :false |
| user      |reference| null :false |foreign_key


