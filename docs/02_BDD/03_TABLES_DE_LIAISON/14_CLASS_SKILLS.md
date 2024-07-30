# 'CLASS_SKILLS' LIASON TABLE

```sql
CREATE TABLE class_skills (
    class_id INT,
    skill_id INT,
    PRIMARY KEY (class_id, skill_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (skill_id) REFERENCES skills(skill_id)
);
```
