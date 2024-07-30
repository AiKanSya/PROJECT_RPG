# 'RACE_ABILITIES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_abilities (
    race_id INT,
    ability_id INT,
    PRIMARY KEY (race_id, ability_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (ability_id) REFERENCES abilities(ability_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_abilities (race_id, ability_id) VALUES (1, 1); -- Dhampire a l'habileté Stealth
INSERT INTO race_abilities (race_id, ability_id) VALUES (2, 2); -- Elf a l'habileté Magic Missile
```
