# 'CLASS_SKILLS' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_skills (
    class_id INT,
    skill_id INT,
    PRIMARY KEY (class_id, skill_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (skill_id) REFERENCES skills(skill_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Compétences pour la classe 1 (Guerrier)
INSERT INTO class_skills (class_id, skill_id)
VALUES (1, (SELECT skill_id FROM skills WHERE skill_name = 'Escape'));

INSERT INTO class_skills (class_id, skill_id)
VALUES (1, (SELECT skill_id FROM skills WHERE skill_name = 'Survival'));

-- Compétence pour la classe 2 (Mage)
INSERT INTO class_skills (class_id, skill_id)
VALUES (2, (SELECT skill_id FROM skills WHERE skill_name = 'Negotiation'));
```
