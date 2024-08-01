# `race_details_view`

### Structure de la Vue :

```sql
CREATE VIEW race_details_view AS
SELECT
    r.id_race,
    r.name AS race_name,
    r.min_height AS min_height,
    r.max_height AS max_height,
    r.min_weight AS min_weight,
    r.max_weight AS max_weight,
    r.base_speed AS base_speed,
    r.min_age AS min_age,
    r.max_age AS max_age,
    r.life_expectancy AS life_expectancy,
    r.is_playable AS is_playable,
    GROUP_CONCAT(DISTINCT l.language_name ORDER BY l.language_name ASC SEPARATOR ', ') AS languages,
    GROUP_CONCAT(DISTINCT rt.racial_type_name ORDER BY rt.racial_type_name ASC SEPARATOR ', ') AS racial_types,
    GROUP_CONCAT(DISTINCT g.gender_type ORDER BY g.gender_type ASC SEPARATOR ', ') AS genders
FROM races r
LEFT JOIN race_languages_junction rl ON r.id_race = rl.id_race
LEFT JOIN languages l ON rl.id_language = l.id_language
LEFT JOIN race_racial_types_junction rrt ON r.id_race = rrt.id_race
LEFT JOIN racial_types rt ON rrt.id_racial_type = rt.id_racial_type
LEFT JOIN race_gender_junction rg ON r.id_race = rg.id_race
LEFT JOIN gender g ON rg.id_gender = g.id_gender
GROUP BY r.id_race;
```
