# 'CHARACTERISTICS' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE characteristics (
    characteristic_id INT AUTO_INCREMENT PRIMARY KEY,
    characteristic_name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO characteristics (characteristic_name) VALUES ('Strength');
INSERT INTO characteristics (characteristic_name) VALUES ('Dexterity');
INSERT INTO characteristics (characteristic_name) VALUES ('Constitution');
INSERT INTO characteristics (characteristic_name) VALUES ('Intelligence');
INSERT INTO characteristics (characteristic_name) VALUES ('Wisdom');
INSERT INTO characteristics (characteristic_name) VALUES ('Charisma');
```
