# 'CLASS_FEATS' LIAISON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_feats (
    class_id INT,
    feat_id INT,
    level INT CHECK (level BETWEEN 1 AND 20),  -- Niveaux de 1 à 20
    PRIMARY KEY (class_id, feat_id, level),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (feat_id) REFERENCES feats(feat_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Insertion des associations classe-dons-niveaux
INSERT INTO class_feats (class_id, feat_id, level) VALUES
(1, (SELECT feat_id FROM feats WHERE feat_name = 'Force surhumaine'), 1),
(1, (SELECT feat_id FROM feats WHERE feat_name = 'Maîtrise des armes lourdes'), 5);
```
