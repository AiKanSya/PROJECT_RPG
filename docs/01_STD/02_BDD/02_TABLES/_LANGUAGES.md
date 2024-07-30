# 'LANGUAGES' TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE languages (
    language_id INT AUTO_INCREMENT PRIMARY KEY,
    language_name VARCHAR(255) NOT NULL,
    description TEXT
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO languages (language_name) VALUES ('Elvish');
INSERT INTO languages (language_name) VALUES ('Common');
INSERT INTO languages (language_name) VALUES ('Dwarvish');
```
