# `races`

### Structure de la Table :

```sql
CREATE TABLE races (
    id_race INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT,
    size_category VARCHAR(10),
    min_height INT,
    max_height INT,
    min_weight INT,
    max_weight INT,
    min_age INT,
    max_age INT,
    lifespan VARCHAR(50),
    speed DECIMAL(5,2),
    languages TEXT,
    racial_types TEXT
);
```

### Insertion des Données (exemple) :

```sql
-- Insertion des races
INSERT INTO races (name, description, size_category, min_height, max_height, min_weight, max_weight, min_age, max_age, lifespan, speed, languages, racial_types) VALUES

('Dhampire', 'Race vampirique avec une longévité immortelle.', 'TP', 160, 190, 60, 90, 12, NULL, 'immortel', 1.5 * 3, 'Commun & Vieux vampirean', 'Humanoïde & Maudit'),

('Drakéide', 'Race draconique avec une force exceptionnelle.', 'TG', 180, 210, 110, 150, 15, 100, 120, 1.5 * 4, 'Commun & Sang-Dragon', 'Humanoïde & Dragon'),

('Elfe', 'Race ancienne avec une grande longévité.', 'M', 150, 180, 50, 80, 100, 600, 750, 1.5 * 3, 'Commun & Eldar', 'Humanoïde & Solarii'),

('Elfe noir', 'Race d’elfe avec une affinité pour la magie noire.', 'M', 150, 180, 50, 80, 100, 600, 750, 1.5 * 3, 'Commun & Eldar', 'Humanoïde & Lunarii'),

('Forgelier', 'Race artificielle créée pour des fins spécifiques.', 'G', 190, 220, 150, 190, 2, NULL, NULL, 1.5 * 3, 'Commun & Synthétique', 'Humanoïde & Artificiel'),

('Golgaut', 'Race géante avec une stature imposante.', 'Gig', 220, 250, 150, 180, 16, 60, 80, 1.5 * 3, 'Commun & Géant', 'Humanoïde & Géant'),

('Humain', 'Race adaptable et commune.', 'M', 160, 190, 50, 90, 16, 50, 60, 1.5 * 3, 'Commun', 'Humanoïde'),

('Kamael', 'Race avec des caractéristiques volantes.', 'M', 160, 190, 50, 80, 16, 60, 80, 1.5 * 3, 'Commun & Volans', 'Humanoïde & Volans'),

('Kijin', 'Race démoniaque avec des pouvoirs tempétueux.', 'M', 160, 190, 60, 90, 16, 800, 1000, 1.5 * 3, 'Commun & Tempestas', 'Humanoïde & Tempestas'),

('Kroot', 'Race avec une nature abérante.', 'M', 180, 210, 90, 125, 16, 60, 75, 1.5 * 3, 'Commun & Kroot', 'Humanoïde & Aberration'),

('Kumiho', 'Race spectrale avec des traits mystiques.', 'M', 160, 190, 50, 90, 16, 800, 1000, 1.5 * 3, 'Commun & Spectral', 'Humanoïde & Spectral'),

('Lamia', 'Race avec des traits mystérieux et mystiques.', 'M', 160, 190, 50, 90, 16, 60, 75, 1.5 * 3, 'Commun & Spectral', 'Humanoïde & Spectral'),

('Lyn', 'Race agile et adaptable.', 'M', 150, 180, 60, 80, 40, 300, 350, 1.5 * 3, 'Commun', 'Humanoïde'),

('Nain', 'Race robuste avec une constitution solide.', 'TP', 120, 150, 50, 90, 50, 300, 350, 1.5 * 3, 'Commun & Nanique', 'Humanoïde'),

('Ork', 'Race brutale avec une forte constitution.', 'M', 180, 210, 90, 125, 16, 60, 75, 1.5 * 3, 'Commun & Ork', 'Humanoïde'),

('Qunari', 'Race imposante avec des capacités magiques et martiales.', 'G', 220, 250, 150, 200, 16, 60, 75, 1.5 * 3, 'Commun & Abyssal', 'Humanoïde & Abyssal'),

('Skitarii', 'Race cybernétique avec des aptitudes uniques.', 'G', 180, 210, 90, 125, 16, 60, 80, 1.5 * 3, 'Commun & Synthétique', 'Humanoïde & Synthétique'),

('Succube', 'Race démoniaque avec des pouvoirs infernaux.', 'M', 170, 200, 70, 110, 16, 90, 100, 1.5 * 3, 'Commun & Infernal', 'Humanoïde & Infernal'),

('Thériantrope', 'Race avec des traits bestiaux et mystiques.', 'M', 160, 190, 60, 90, 16, 60, 75, 1.5 * 3, 'Commun & Thériantrope', 'Humanoïde & Bête'),
```
