# 'RACE_SIZE_CATEGORIES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_size_categories (
    race_id INT,
    size_id INT,
    PRIMARY KEY (race_id, size_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (size_id) REFERENCES size_categories(size_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_size_categories (race_id, size_id) VALUES (1, 2); -- Dhampire est de taille Moyenne
INSERT INTO race_size_categories (race_id, size_id) VALUES (2, 2); -- Elf est de taille Moyenne
INSERT INTO race_size_categories (race_id, size_id) VALUES (2, 3); -- Elf peut aussi être de grande taille
```
