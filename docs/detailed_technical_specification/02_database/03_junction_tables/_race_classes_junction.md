# `race_classes_junction`

### Structure de la Table :

```sql
CREATE TABLE race_classes_junction (
    id_race INT,
    id_class INT,
    FOREIGN KEY (id_race) REFERENCES races(id_race),
    FOREIGN KEY (id_class) REFERENCES classes(id_class),
    PRIMARY KEY (id_race, id_class)
);
```

### Insertion des Données (exemple) :

```sql
-- Insertion des relations entre les races et les classes
INSERT INTO race_classes_junction (id_race, id_class) VALUES
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Dhampire'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Drakéide'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Elfe'), (SELECT id_class FROM classes WHERE name = 'Ranger')),

((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Elfe noir'), (SELECT id_class FROM classes WHERE name = 'Ranger')),

((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Forgelier'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Golgaut'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),
((SELECT id_race FROM races WHERE name = 'Humain'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),
((SELECT id_race FROM races WHERE name = 'Kamael'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Kijin'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Kroot'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Kumiho'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Lamia'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Lyn'), (SELECT id_class FROM classes WHERE name = 'Ranger')),

((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Nain'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),

((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Ork'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Qunari'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Inquisitor')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Redemptor')),
((SELECT id_race FROM races WHERE name = 'Skitarii'), (SELECT id_class FROM classes WHERE name = 'Technaugure')),

((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Ranger')),
((SELECT id_race FROM races WHERE name = 'Succube'), (SELECT id_class FROM classes WHERE name = 'Sorcier')),

((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Adepte')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Assassin')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Berzerker')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Chaman')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Guerrier')),
((SELECT id_race FROM races WHERE name = 'Thériantrope'), (SELECT id_class FROM classes WHERE name = 'Ranger'));
```
