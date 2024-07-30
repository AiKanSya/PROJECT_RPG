# 'CLASS_SAVE_THROWS' LIASON TABLE

```sql
CREATE TABLE class_save_throws (
    class_id INT,
    characteristic_id INT,
    PRIMARY KEY (class_id, characteristic_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (characteristic_id) REFERENCES characteristics(characteristic_id)
);
```
