# 'RACE_SKILL_ADVANTAGES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_skill_advantages (
    race_id INT,
    skill_id INT,
    advantage_value INT,
    PRIMARY KEY (race_id, skill_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (skill_id) REFERENCES skills(skill_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_skill_advantages (race_id, skill_id, advantage_value) VALUES (1, 1, 5); -- Dhampire a un avantage de 5 dans Arcana
INSERT INTO race_skill_advantages (race_id, skill_id, advantage_value) VALUES (1, 2, 3); -- Dhampire a un avantage de 3 dans Stealth
INSERT INTO race_skill_advantages (race_id, skill_id, advantage_value) VALUES (2, 3, 7); -- Elf a un avantage de 7 dans Negociation
```
