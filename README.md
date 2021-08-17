# テーブル設計

## users テーブル

| Column             | type   | Options                |
| ------------------ | ------ | ---------------------- |
| encrypted_password | string | NOT NULL               |
| email              | string | NOT NULL, unique: true |
| name               | string | NOT NULL               |
| phone              | string | NOT NULL               |
| address            | string | NOT NULL               |

### Association

- has_many :orders
- has_one :reservation