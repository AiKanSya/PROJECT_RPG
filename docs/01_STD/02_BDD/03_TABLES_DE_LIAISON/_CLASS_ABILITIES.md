# 'CLASS_ABILITIES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_abilities (
    class_id INT,
    ability_id INT,
    PRIMARY KEY (class_id, ability_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (ability_id) REFERENCES abilities(ability_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO class_abilities (class_id, ability_id) VALUES (1, 1); -- Warrior classe a l'habileté Stealth
INSERT INTO class_abilities (class_id, ability_id) VALUES (2, 2); -- Mage classe a l'habileté Magic Missile
```
