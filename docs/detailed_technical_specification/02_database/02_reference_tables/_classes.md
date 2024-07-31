# `classes`

### Structure de la Table :

```sql
CREATE TABLE classes (
    id_class INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO classes (name) VALUES
('Adepte'),
('Assassin'),
('Berzerker'),
('Chaman'),
('Guerrier'),
('Inquisitor'),
('Ranger'),
('Redemptor'),
('Sorcier'),
('Technaugure');
```
