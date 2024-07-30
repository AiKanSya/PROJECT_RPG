# 'CHARACTERISTICS' TABLE

```sql
CREATE TABLE characteristics (
    characteristic_id INT AUTO_INCREMENT PRIMARY KEY,
    characteristic_name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT
);
```
