# テーブル設計

## usersテーブル

| Column                | Type       | options                   |
| --------------------- | ---------- | ------------------------- |
| name                  | string     | null: false               |
| email                 | string     | null: false, unique: true |
| encrypted_password    | string     | null: false               |

### Association

- has_many :books