# 'RACE_CHARACTERISTICS_BONUSES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_characteristic_bonuses (
    race_id INT,
    characteristic_id INT,
    bonus_value INT NOT NULL,
    PRIMARY KEY (race_id, characteristic_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (characteristic_id) REFERENCES characteristics(characteristic_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Bonus pour la race 1 (Elfe) en Dextérité
INSERT INTO race_characteristic_bonuses (race_id, characteristic_id, bonus_value)
VALUES (1, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Dexterity'), 2);

-- Malus pour la race 1 (Elfe) en Constitution
INSERT INTO race_characteristic_bonuses (race_id, characteristic_id, bonus_value)
VALUES (1, (SELECT characteristic_id FROM characteristics WHERE characteristic_name = 'Constitution'), -1);
```
