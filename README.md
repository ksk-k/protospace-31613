usersテーブル

| Column     | Type   | Options  | 
| ---------- | ------ | -------- |
| email      | string | not null |
| password   | string | not null |
| name       | string | not null |
| profile    | text   | not nill |
| occupation | text   | not null |
| position   | text   | not null |


prototypesテーブル

| Column     | Type      | Options            | 
| ---------- | --------- | ------------------ |
| title      | string    | not null           |
| catch_copy | text      | not null           |
| concept    | text      | not null           |
| image      |           | ActiveStorageで実装 |
| user       | reference | not null           |


commentsテーブル

| Column    | Type      | Options  | 
| --------- | --------- | -------- |
| text      | text      | not null |
| user      | reference |          |
| prototype | reference |          |