# 'RACE_LANGUAGES' LIASON TABLE

```sql
CREATE TABLE race_languages (
    race_id INT,
    language_id INT,
    PRIMARY KEY (race_id, language_id),
    FOREIGN KEY (race_id) REFERENCES races(race_id),
    FOREIGN KEY (language_id) REFERENCES languages(language_id)
);
```
