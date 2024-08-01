# `races`

### Structure de la Table :

```sql
CREATE TABLE races (
    id_race INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    min_height INT NOT NULL,
    max_height INT NOT NULL,
    min_weight INT NOT NULL,
    max_weight INT NOT NULL,
    base_speed DECIMAL(5, 2) NOT NULL,
    min_age INT NOT NULL,
    max_age INT,
    life_expectancy INT,
    is_playable BOOLEAN NOT NULL,
    category_size VARCHAR(50) NOT NULL,
    gender_type VARCHAR(50) NOT NULL,
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
-- Insertion des races
INSERT INTO races (name, min_height, max_height, min_weight, max_weight, base_speed, min_age, max_age, life_expectancy, is_playable, category_size, gender_type)
VALUES
    ('Dhampire', 160, 190, 60, 90, 9.0, 12, NULL, NULL, TRUE, 'M', 'Male/Female'),
    ('Drakéide', 180, 210, 110, 150, 9.0, 15, 100, 120, TRUE, 'M', 'Male/Female'),
    ('Elfe', 150, 180, 50, 80, 9.0, 100, 600, 750, TRUE, 'M', 'Male/Female'),
    ('Elfe noir', 150, 180, 50, 80, 9.0, 100, 600, 750, TRUE, 'M', 'Male/Female'),
    ('Forgelier', 190, 220, 150, 190, 9.0, 2, NULL, NULL, TRUE, 'G', 'Asexué'),
    ('Golgaut', 220, 250, 150, 180, 9.0, 16, 60, 80, TRUE, 'G', 'Male'),
    ('Humain', 160, 190, 50, 90, 9.0, 16, 50, 60, TRUE, 'M', 'Male/Female'),
    ('Kamael', 160, 190, 50, 80, 9.0, 16, 60, 80, TRUE, 'M', 'Male/Female'),
    ('Kijin', 160, 190, 50, 80, 9.0, 20, 800, 1000, TRUE, 'M', 'Male/Female'),
    ('Kroot', 180, 210, 90, 125, 9.0, 16, 60, 75, TRUE, 'M', 'Asexué'),
    ('Kumiho', 160, 190, 50, 90, 9.0, 16, 800, 1000, TRUE, 'M', 'Female'),
    ('Lyn', 150, 180, 60, 80, 9.0, 40, 300, 350, TRUE, 'M', 'Male/Female'),
    ('Nain', 120, 150, 50, 90, 9.0, 50, 300, 350, TRUE, 'M', 'Male/Female'),
    ('Ork', 180, 210, 90, 125, 9.0, 16, 60, 75, TRUE, 'M', 'Male/Female'),
    ('Qunari', 200, 230, 100, 140, 9.0, 30, 60, 75, TRUE, 'G', 'Male'),
    ('Skitarii', 160, 190, 50, 90, 9.0, 16, 50, 60, TRUE, 'M', 'Male/Female'),
    ('Succube', 170, 200, 70, 110, 9.0, 16, 90, 100, TRUE, 'M', 'Female'),
    ('Thériantrope', 160, 200, 50, 90, 9.0, 16, 60, 75, TRUE, 'M', 'Male/Female'),
    ('Lamia', 160, 190, 50, 90, 9.0, 16, 60, 75, TRUE, 'M', 'Female');

```
