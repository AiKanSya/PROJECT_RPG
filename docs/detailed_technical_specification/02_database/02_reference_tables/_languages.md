# `languages`

### Structure de la Table :

```sql
CREATE TABLE languages (
    id_language INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO languages (name) VALUES
('Abyssal'),
('Commun'),
('Eldar'),
('Géant'),
('Infernal'),
('Kroot'),
('Nanique'),
('Ophikin'),
('Sang-Dragon'),
('Spectral'),
('Synthétique'),
('Tempestas'),
('Thériantrope'),
('Vieux vampirean');
```
