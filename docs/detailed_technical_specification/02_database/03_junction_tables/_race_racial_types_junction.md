# `race_racial_types_junction`

### Structure de la Table :

```sql
CREATE TABLE race_racial_types_junction (
    id_race INT,
    id_racial_type INT,
    FOREIGN KEY (id_race) REFERENCES races(id_race),
    FOREIGN KEY (id_racial_type) REFERENCES racial_types(id_racial_type),
    PRIMARY KEY (id_race, id_racial_type)
);
```

### Insertion des Données (exemple) :

```sql
-- Insérer les données dans race_racial_types_junction
INSERT INTO race_racial_types_junction (id_race, id_racial_type) VALUES
-- Dhampire
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_racial_type FROM racial_types WHERE name = 'Maudit')),

-- Drakéide
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_racial_type FROM racial_types WHERE name = 'Dragon')),

-- Elfe
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_racial_type FROM racial_types WHERE name = 'Solarii')),

-- Elfe noir
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_racial_type FROM racial_types WHERE name = 'Lunarii')),

-- Forgelier
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_racial_type FROM racial_types WHERE name = 'Artificiel')),

-- Golgaut
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_racial_type FROM racial_types WHERE name = 'Géant')),

-- Humain
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),

-- Kamael
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_racial_type FROM racial_types WHERE name = 'Volans')),

-- Kijin
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_racial_type FROM racial_types WHERE name = 'Tempestas')),

-- Kroot
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_racial_type FROM racial_types WHERE name = 'Aberration')),

-- Kumiho
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_racial_type FROM racial_types WHERE name = 'Spectral')),

-- Lamia
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_racial_type FROM racial_types WHERE name = 'Abomination'));

-- Lyn
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),

-- Nain
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),

-- Ork
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_racial_type FROM racial_types WHERE name = 'Ork')),

-- Qunari
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_racial_type FROM racial_types WHERE name = 'Abyssal')),

-- Skitarii
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_racial_type FROM racial_types WHERE name = 'Synthétique')),

-- Succube
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_racial_type FROM racial_types WHERE name = 'Infernal')),

-- Thériantrope
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_racial_type FROM racial_types WHERE name = 'Humanoïde')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_racial_type FROM racial_types WHERE name = 'Bête')),
```
