# 'HIT_DICE_TYPES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE hit_dice_types (
    hit_dice_id INT AUTO_INCREMENT PRIMARY KEY,
    hit_dice_name VARCHAR(10) NOT NULL UNIQUE, -- Par exemple 'D4', 'D6', 'D8', 'D10', 'D12'
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D4');
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D6');
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D8');
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D10');
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D12');
INSERT INTO hit_dice_types (hit_dice_name) VALUES ('D20');
```
