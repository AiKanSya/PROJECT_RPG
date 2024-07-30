# 'RACE_TYPES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_types (
    race_id INT,
    type_id INT,
    PRIMARY KEY (race_id, type_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (type_id) REFERENCES types(type_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_types (race_id, type_id) VALUES (1, 1); -- Dhampire est Humanoide
INSERT INTO race_types (race_id, type_id) VALUES (1, 2); -- Dhampire est Mort-vivant
INSERT INTO race_types (race_id, type_id) VALUES (2, 1); -- Elf est Humanoide
INSERT INTO race_types (race_id, type_id) VALUES (2, 3); -- Elf est Magique
```
