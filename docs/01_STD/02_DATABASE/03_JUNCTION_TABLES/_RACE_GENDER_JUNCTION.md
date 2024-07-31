# `race_languages_junction`

### Structure de la Table :

```sql
CREATE TABLE race_gender_junction (
    id_race INT,
    id_gender INT,
    PRIMARY KEY (id_race, id_gender),
    FOREIGN KEY (id_race) REFERENCES races(id_race),
    FOREIGN KEY (id_gender) REFERENCES gender(id_gender)
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO race_gender_junction (id_race, id_gender) VALUES
-- Dhampire
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Drakéide
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Elfe
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Elfe noir
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Forgelier
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_gender FROM gender WHERE gender_type = 'Asexual')),

-- Golgaut
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),

-- Humain
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Kamael
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Kijin
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Kroot
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_gender FROM gender WHERE gender_type = 'Asexual')),

-- Kumiho
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Lamia
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Lyn
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Nain
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Ork
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Qunari
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),

-- Skitarii
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Succube
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_gender FROM gender WHERE gender_type = 'Female')),

-- Thériantrope
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_gender FROM gender WHERE gender_type = 'Male')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_gender FROM gender WHERE gender_type = 'Female'));
```
