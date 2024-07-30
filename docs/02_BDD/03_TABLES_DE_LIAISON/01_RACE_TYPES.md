# 'RACE_TYPES' LIASON TABLE

```sql
CREATE TABLE race_types (
    race_id INT,
    type_id INT,
    PRIMARY KEY (race_id, type_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (type_id) REFERENCES types(type_id)
);
```
