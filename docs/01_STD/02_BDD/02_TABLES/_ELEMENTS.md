# 'ELEMENTS' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE elements (
    element_id INT AUTO_INCREMENT PRIMARY KEY,
    element_name VARCHAR(255) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO elements (element_name) VALUES ('Sacré');
INSERT INTO elements (element_name) VALUES ('Feu');
INSERT INTO elements (element_name) VALUES ('Eau');
```
