# 'RACE_ABILITIES' LIASON TABLE

```sql
CREATE TABLE race_abilities (
    race_id INT,
    ability_id INT,
    PRIMARY KEY (race_id, ability_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (ability_id) REFERENCES abilities(ability_id)
);
```
