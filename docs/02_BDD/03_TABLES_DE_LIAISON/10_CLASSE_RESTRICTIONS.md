# 'RACE_CLASS_RESTRICTIONS' LIASON TABLE

```sql
CREATE TABLE race_class_restrictions (
    race_id INT,
    class_id INT,
    restriction_type ENUM('Allowed', 'Not Allowed') NOT NULL,
    PRIMARY KEY (race_id, class_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id)
);
```
