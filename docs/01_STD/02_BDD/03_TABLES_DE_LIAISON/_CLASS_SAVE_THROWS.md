# 'CLASS_SAVE_THROWS' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_save_throws (
    class_id INT,
    characteristic_id INT,
    PRIMARY KEY (class_id, characteristic_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (characteristic_id) REFERENCES characteristics(characteristic_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Jets de sauvegarde avantagés pour la classe 1 (Guerrier)
INSERT INTO class_save_throws (class_id, characteristic_id)
VALUES (1, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Strength'));

INSERT INTO class_save_throws (class_id, characteristic_id)
VALUES (1, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Constitution'));

-- Jets de sauvegarde avantagés pour la classe 2 (Mage)
INSERT INTO class_save_throws (class_id, characteristic_id)
VALUES (2, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Intelligence'));

INSERT INTO class_save_throws (class_id, characteristic_id)
VALUES (2, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Wisdom'));
```
