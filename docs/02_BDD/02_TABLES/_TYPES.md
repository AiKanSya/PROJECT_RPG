# 'TYPES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE types (
    type_id INT AUTO_INCREMENT PRIMARY KEY,
    type_name VARCHAR(255) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO types (type_name) VALUES ('Humanoide');
INSERT INTO types (type_name) VALUES ('Mort-vivant');
INSERT INTO types (type_name) VALUES ('Magique');
```
