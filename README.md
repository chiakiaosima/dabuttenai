# テーブル設計

## usersテーブル

| Column                | Type       | options                   |
| --------------------- | ---------- | ------------------------- |
| nick_name             | string     | null: false               |
| email                 | string     | null: false, unique: true |
| encrypted_password    | string     | null: false               |

### Association

- has_many :books

## booksテーブル

| Column                | Type           | options                   |
| --------------------- | -------------- | ------------------------- |
| book_name             | string         | null: false               |
| user                  | references     | null: false, unique: true |

### Association
　
- belongs_to :user