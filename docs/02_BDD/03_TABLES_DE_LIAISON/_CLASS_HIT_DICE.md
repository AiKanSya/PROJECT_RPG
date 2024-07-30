# 'CLASS_HIT_DICE' LIAISON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_hit_dice (
    class_id INT,
    hit_dice_id INT,
    PRIMARY KEY (class_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (hit_dice_id) REFERENCES hit_dice_types(hit_dice_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Dé de vie pour la classe 1 (Guerrier)
INSERT INTO class_hit_dice (class_id, hit_dice_id)
VALUES (1, (SELECT hit_dice_id FROM hit_dice_types WHERE hit_dice_name = 'D12'));

-- Dé de vie pour la classe 2 (Mage)
INSERT INTO class_hit_dice (class_id, hit_dice_id)
VALUES (2, (SELECT hit_dice_id FROM hit_dice_types WHERE hit_dice_name = 'D4'));
```
