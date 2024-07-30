# 'OBJETC_CATEGORIES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE object_categories (
    object_category_id INT AUTO_INCREMENT PRIMARY KEY,
    object_category_name VARCHAR(100) NOT NULL UNIQUE,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO object_categories (object_category_name) VALUES ('Two-Handed Sword');
INSERT INTO object_categories (object_category_name) VALUES ('Leather Armor');
INSERT INTO object_categories (object_category_name) VALUES ('Staff');
```
