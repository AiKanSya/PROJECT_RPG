# 'ABILITIES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE abilities (
    ability_id INT AUTO_INCREMENT PRIMARY KEY,
    ability_name VARCHAR(50) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO abilities (ability_name, description) VALUES ('Stealth', 'Ability to move silently and hide effectively.');
INSERT INTO abilities (ability_name, description) VALUES ('Magic Missile', 'Cast a magical missile that never misses.');
```
