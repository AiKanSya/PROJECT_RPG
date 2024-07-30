# 'CLASSES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE classes (
    class_id INT AUTO_INCREMENT PRIMARY KEY,
    class_name VARCHAR(50) NOT NULL,
    description TEXT,
    playable BOOLEAN NOT NULL DEFAULT FALSE -- Indique si la classe est jouable ou non
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO classes (class_name, description, playable) VALUES ('Warrior', 'A strong and skilled fighter.', TRUE);
INSERT INTO classes (class_name, description, playable) VALUES ('Mage', 'A master of magical arts.', TRUE);
INSERT INTO classes (class_name, description, playable) VALUES ('Rogue', 'A stealthy and agile character.', TRUE);
INSERT INTO classes (class_name, description, playable) VALUES ('Necromancer', 'A dark magic user.', FALSE); -- Exemple de classe non jouable
```
