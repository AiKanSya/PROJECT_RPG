# 'SIZE_CATEGORIES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE size_categories (
    size_id INT AUTO_INCREMENT PRIMARY KEY,
    size_cat VARCHAR(10) NOT NULL,
    size_name VARCHAR(255),
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO size_categories (size_cat, size_name, description) VALUES ('P', 'De petite taille, moins de 1 mètre.');
INSERT INTO size_categories (size_cat, size_name, description) VALUES ('M', 'De taille moyenne, entre 1 et 2 mètres.');
INSERT INTO size_categories (size_cat, size_name, description) VALUES ('G', 'De grande taille, plus de 2 mètres.');
```
