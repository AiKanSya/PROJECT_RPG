# 'PROFICIENCY_BONUS_LEVELS' LIAISON TABLE

```sql
CREATE TABLE proficiency_bonus_levels (
    proficiency_bonus_level_id INT AUTO_INCREMENT PRIMARY KEY,
    class_id INT,
    level INT CHECK (level BETWEEN 1 AND 20),  -- Niveaux de 1 à 20
    proficiency_bonus INT NOT NULL,           -- Bonus de maîtrise pour ce niveau
    FOREIGN KEY (class_id) REFERENCES classes(class_id)
);
```
