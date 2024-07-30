# 'RACE_CHARACTERISTICS_BONUSES' LIASON TABLE

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
