# `race_languages_junction`

### Structure de la Table :

```sql
CREATE TABLE race_languages_junction (
    id_race INT,
    id_language INT,
    PRIMARY KEY (id_race, id_language),
    FOREIGN KEY (id_race) REFERENCES races(id_race) ON DELETE CASCADE,
    FOREIGN KEY (id_language) REFERENCES languages(id_language) ON DELETE CASCADE
);
```

### Insertion des Données (exemple) :

```sql
-- Insérer les données dans race_languages_junction
INSERT INTO race_languages_junction (id_race, id_language) VALUES
-- Dhampire
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_language FROM languages WHERE name = 'Vieux vampirean')),

-- Drakéide
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_language FROM languages WHERE name = 'Sang-Dragon')),

-- Elfe
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_language FROM languages WHERE name = 'Eldar')),

-- Elfe noir
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_language FROM languages WHERE name = 'Eldar')),

-- Forgelier
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_language FROM languages WHERE name = 'Synthétique')),

-- Golgaut
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_language FROM languages WHERE name = 'Géant')),

-- Humain
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_language FROM languages WHERE name = 'Commun')),

-- Kamael
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_language FROM languages WHERE name = 'Volans')),

-- Kijin
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_language FROM languages WHERE name = 'Tempestas')),

-- Kroot
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_language FROM languages WHERE name = 'Kroot')),

-- Kumiho
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_language FROM languages WHERE name = 'Spectral')),

-- Lamia
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_language FROM languages WHERE name = 'Ophikin'));

-- Lyn
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_language FROM languages WHERE name = 'Commun')),

-- Nain
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_language FROM languages WHERE name = 'Nanique')),

-- Ork
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_language FROM languages WHERE name = 'Ork')),

-- Qunari
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_language FROM languages WHERE name = 'Abyssal')),

-- Skitarii
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_language FROM languages WHERE name = 'Synthétique')),

-- Succube
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_language FROM languages WHERE name = 'Infernal')),

-- Thériantrope
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_language FROM languages WHERE name = 'Commun')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_language FROM languages WHERE name = 'Thériantrope')),
```
