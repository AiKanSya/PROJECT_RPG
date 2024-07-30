# 'SKILLS' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE skills (
    skill_id INT AUTO_INCREMENT PRIMARY KEY,
    skill_name VARCHAR(50) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO skills (skill_name) VALUES ('Arcana');
INSERT INTO skills (skill_name) VALUES ('Stealth');
INSERT INTO skills (skill_name) VALUES ('Negociation');
INSERT INTO skills (skill_name) VALUES ('Escape');
INSERT INTO skills (skill_name) VALUES ('Negotiation');
INSERT INTO skills (skill_name) VALUES ('Survival');
```
