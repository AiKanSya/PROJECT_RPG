# 'CLASS_ABILITIES' LIASON TABLE

```sql
CREATE TABLE class_abilities (
    class_id INT,
    ability_id INT,
    PRIMARY KEY (class_id, ability_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (ability_id) REFERENCES abilities(ability_id)
);
```
