# 'RACE_SKILL_DISADVANTAGES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_skill_disadvantages (
    race_id INT,
    skill_id INT,
    disadvantage_value INT,
    PRIMARY KEY (race_id, skill_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (skill_id) REFERENCES skills(skill_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_skill_disadvantages (race_id, skill_id, disadvantage_value) VALUES (1, 3, 4); -- Dhampire a un désavantage de 4 dans Negociation
INSERT INTO race_skill_disadvantages (race_id, skill_id, disadvantage_value) VALUES (2, 2, 2); -- Elf a un désavantage de 2 dans Stealth
```
