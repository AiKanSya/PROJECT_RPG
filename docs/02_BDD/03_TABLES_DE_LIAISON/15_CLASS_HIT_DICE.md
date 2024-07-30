# 'CLASS_HIT_DICE' LIAISON TABLE

```sql
CREATE TABLE class_hit_dice (
    class_id INT,
    hit_dice_id INT,
    PRIMARY KEY (class_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (hit_dice_id) REFERENCES hit_dice_types(hit_dice_id)
);
```
