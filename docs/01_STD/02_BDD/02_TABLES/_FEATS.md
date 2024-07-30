# 'FEATS' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE feats (
    feat_id INT AUTO_INCREMENT PRIMARY KEY,
    feat_name VARCHAR(50) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Insertion des dons
INSERT INTO feats (feat_name, description) VALUES
('Force surhumaine', 'Augmente la force du personnage.'),
('Maîtrise des armes lourdes', 'Permet l’utilisation experte des armes lourdes.');
```
