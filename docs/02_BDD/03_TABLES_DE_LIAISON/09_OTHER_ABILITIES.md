# 'OTHER_ABILITIES' LIASON TABLE

```sql
CREATE TABLE other_abilities (
    aspect_name VARCHAR(50),  -- Nom de l'aspect auquel l'habileté est liée
    ability_id INT,
    PRIMARY KEY (aspect_name, ability_id),
    FOREIGN KEY (ability_id) REFERENCES abilities(ability_id)
);
```
