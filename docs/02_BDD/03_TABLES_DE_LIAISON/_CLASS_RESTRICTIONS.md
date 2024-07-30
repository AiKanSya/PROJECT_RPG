# 'RACE_CLASS_RESTRICTIONS' LIASON TABLE

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
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (1, 1, 'Allowed'); -- Dhampire peut être Warrior
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (1, 2, 'Not Allowed'); -- Dhampire ne peut pas être Mage
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (2, 2, 'Allowed'); -- Elf peut être Mage
INSERT INTO race_class_restrictions (race_id, class_id, restriction_type) VALUES (2, 3, 'Allowed'); -- Elf peut être Rogue
```
