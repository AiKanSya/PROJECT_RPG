# 'HIT_DICE_TYPES' TABLE

```sql
CREATE TABLE hit_dice_types (
    hit_dice_id INT AUTO_INCREMENT PRIMARY KEY,
    hit_dice_name VARCHAR(10) NOT NULL UNIQUE, -- Par exemple 'D4', 'D6', 'D8', 'D10', 'D12'
    description TEXT
);
```
