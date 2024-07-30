# 'OBJETC_CATEGORIES' TABLE

```sql
CREATE TABLE object_categories (
    object_category_id INT AUTO_INCREMENT PRIMARY KEY,
    object_category_name VARCHAR(100) NOT NULL UNIQUE,
    description TEXT
);
```
