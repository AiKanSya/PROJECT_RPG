# `race_racial_abilities_junction`

### Structure de la Table :

```sql
CREATE TABLE race_racial_abilities_junction (
    id_race INT,
    id_racial_ability INT,
    PRIMARY KEY (id_race, id_racial_ability),
    FOREIGN KEY (id_race) REFERENCES races(id_race) ON DELETE CASCADE,
    FOREIGN KEY (id_racial_ability) REFERENCES racial_abilities(id_racial_ability) ON DELETE CASCADE
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO race_racial_abilities_junction (id_race, id_racial_ability) VALUES

-- Dhampire
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Vision dans le noir')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Regénération rapide')),

-- Elfe
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Vision nocturne')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Sens aiguisés')),

-- Drakéide
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Résistance au feu')),

-- Goliath
((SELECT id_race FROM races WHERE name = 'Goliath'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Agilité accrue')),

-- Loxodon
((SELECT id_race FROM races WHERE name = 'Loxodon'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Détection des présences')),

-- Kumiho
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Sens aiguisés')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_racial_ability FROM racial_abilities WHERE name = 'Immunité aux poisons'));
```
