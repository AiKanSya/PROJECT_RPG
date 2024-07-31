# `size_categories`

### Structure de la Table :

```sql
CREATE TABLE size_categories (
    id_size_category INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    description VARCHAR(100) NOT NULL,
    space VARCHAR(20) NOT NULL
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO size_categories (name, description, space) VALUES

('TP', 'Très petite', '75 cm x 75 cm'),
('P', 'Petite', '150 cm x 150 cm'),
('M', 'Moyenne', '150 cm x 150 cm'),
('G', 'Grande', '3 m x 3 m'),
('TG', 'Très grande', '4.5 m x 4.5 m'),
('Gig', 'Gigantesque', '6 m x 6 m');
```
