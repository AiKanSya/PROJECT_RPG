# 'RACE_CLASS_RESTRICTION' LIAISON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_class_restrictions (
    race_id INT,
    class_id INT,
    restriction_type ENUM('Allowed', 'Not Allowed') NOT NULL,
    PRIMARY KEY (race_id, class_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (1, 1, 'Allowed'); -- Race 1 peut choisir la classe 1
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (1, 2, 'Not Allowed'); -- Race 1 ne peut pas choisir la classe 2
```
