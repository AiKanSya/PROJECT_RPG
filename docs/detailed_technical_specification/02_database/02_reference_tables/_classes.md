# `classes`

### Structure de la Table :

```sql
CREATE TABLE classes (
    id_class INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    is_playable BOOLEAN NOT NULL,
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO classes (name, is_playable)
VALUES
    ('Adepte', TRUE),
    ('Assassin', TRUE),
    ('Berzerker', TRUE),
    ('Chaman', TRUE),
    ('Guerrier', TRUE),
    ('Inquisitor', TRUE),
    ('Ranger', TRUE),
    ('Redemptor', TRUE),
    ('Sorcier', TRUE),
    ('Technaugure', TRUE);
```
