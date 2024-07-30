# 'RACE_LANGUAGES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE race_languages (
    race_id INT,
    language_id INT,
    PRIMARY KEY (race_id, language_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (language_id) REFERENCES languages(language_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO race_languages (race_id, language_id) VALUES (1, 1); -- Dhampire connaît Elvish
INSERT INTO race_languages (race_id, language_id) VALUES (1, 2); -- Dhampire connaît Common
INSERT INTO race_languages (race_id, language_id) VALUES (2, 1); -- Elf connaît Elvish
INSERT INTO race_languages (race_id, language_id) VALUES (2, 3); -- Elf connaît Dwarvish
```
