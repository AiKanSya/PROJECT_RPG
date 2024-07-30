# 'RACES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE races (
    race_id INT AUTO_INCREMENT PRIMARY KEY,
    race_name VARCHAR(255) NOT NULL,
    description TEXT,
    playable BOOLEAN NOT NULL DEFAULT FALSE,
    specific_size VARCHAR(255),
    speed DECIMAL(5, 1),
    min_age INT,
    max_age INT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO races (race_name, description, playable, specific_size, speed, min_age, max_age) VALUES ('Dhampire', 'A half-vampire, half-human hybrid.', TRUE, '160 à 190 cm', 9.0, 18, 150);
INSERT INTO races (race_name, description, playable, specific_size, speed, min_age, max_age) VALUES ('Elf', 'A race of magical humanoids.', TRUE, '150 à 180 cm', 12.0, 100, 700);
```
