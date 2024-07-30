# 'SIZE_CATEGORIES' TABLE

```sql
CREATE TABLE size_categories (
    size_id INT AUTO_INCREMENT PRIMARY KEY,
    size_cat VARCHAR(10) NOT NULL,
    size_name VARCHAR(255),
    description TEXT
);
```
