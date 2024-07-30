# 'PROFICIENCY_BONUS_LEVELS' LIAISON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE proficiency_bonus_levels (
    proficiency_bonus_level_id INT AUTO_INCREMENT PRIMARY KEY,
    class_id INT,
    level INT CHECK (level BETWEEN 1 AND 20),  -- Niveaux de 1 à 20
    proficiency_bonus INT NOT NULL,           -- Bonus de maîtrise pour ce niveau
    FOREIGN KEY (class_id) REFERENCES classes(class_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Exemple d'insertion des bonus de maîtrise pour la classe Guerrier (class_id = 1)
INSERT INTO proficiency_bonus_levels (class_id, level, proficiency_bonus)
VALUES
    (1, 1, 2),
    (1, 2, 2),
    (1, 3, 2),
    (1, 4, 3),
    (1, 5, 3),
    (1, 6, 3),
    (1, 7, 4),
    (1, 8, 4),
    (1, 9, 4),
    (1, 10, 5),
    (1, 11, 5),
    (1, 12, 5),
    (1, 13, 6),
    (1, 14, 6),
    (1, 15, 6),
    (1, 16, 6),
    (1, 17, 6),
    (1, 18, 6),
    (1, 19, 6),
    (1, 20, 6);
```
