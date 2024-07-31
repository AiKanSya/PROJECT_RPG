# `racial_abilities`

### Structure de la Table :

```sql
CREATE TABLE racial_abilities (
    id_racial_ability INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) NOT NULL UNIQUE,
    description TEXT
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO racial_abilities (name, description) VALUES

('Vision dans le noir', 'Permet de voir dans l’obscurité totale.'),
('Vision nocturne', 'Améliore la vision dans des conditions de faible luminosité.'),
('Résistance au feu', 'Réduit les dégâts causés par les attaques de feu.'),
('Immunité aux poisons', 'Ne subit aucun effet des poisons.'),
('Agilité accrue', 'Augmente la vitesse et la flexibilité des mouvements.'),
('Détection des présences', 'Permet de détecter des présences invisibles ou cachées.'),
('Regénération rapide', 'Accélère la guérison des blessures.'),
('Sens aiguisés', 'Améliore la perception des sons et des mouvements.');
```
