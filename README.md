# テーブル設計

## users テーブル

| Column             | Type   | Options     |
| ------------------ | ------ | ----------- |
| email              | string | null: not   |
| password           | string | null: not   |
| name               | string | null: not   |
| profile            | text   | null: not   |
| occupation         | text   | null: not   |
| position           | text   | null: not   |

## prototypes テーブル

| Column      | Type       | Options     |
| ------      | ------     | ----------- |
| title       | string     | null: not   |
| catch_copy  | text       | null: not   |
| concept     | text       | null: not   |
| user        | references | null: false |

## comments テーブル

| Column      | Type       | Options     |
| ------      | ------     | ----------- |
| text        | text       | null: not   |
| user        | references | null: false |
| prototype   | references | null: false |

