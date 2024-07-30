# 'RACE_SKILL_DISADVANTAGES' LIASON TABLE

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
