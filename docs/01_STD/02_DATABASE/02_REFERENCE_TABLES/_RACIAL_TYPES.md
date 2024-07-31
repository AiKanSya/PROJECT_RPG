# `racial_types`

### Structure de la Table :

```sql
CREATE TABLE racial_types (
    id_racial_type INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO racial_types (name) VALUES
('Abomination'),
('Artificiel'),
('Abyssal'),
('Bête'),
('Dragon'),
('Géant'),
('Humanoïde'),
('Infernal'),
('Lunarii'),
('Maudit'),
('Spectral'),
('Solarii'),
('Synthétique'),
('Tempestas'),
('Volans');
```
