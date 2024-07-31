# `gender`

### Structure de la Table :

```sql
CREATE TABLE gender (
    id_gender INT AUTO_INCREMENT PRIMARY KEY,
    gender_type VARCHAR(50) NOT NULL UNIQUE
);
```

### Insertion des Données (exemple) :

```sql
INSERT INTO gender (gender_type) VALUES
('Male'),
('Female'),
('Asexual');
```
