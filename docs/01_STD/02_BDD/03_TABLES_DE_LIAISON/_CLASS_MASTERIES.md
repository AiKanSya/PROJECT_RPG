# 'CLASS_MASTERIES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE class_masteries (
    class_id INT,
    object_category_id INT,
    PRIMARY KEY (class_id, object_category_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (object_category_id) REFERENCES object_categories(object_category_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
-- Maîtrises pour la classe 1 (Guerrier)
INSERT INTO class_masteries (class_id, object_category_id)
VALUES (1, (SELECT object_category_id FROM object_categories WHERE object_category_name = 'Two-Handed Sword'));

INSERT INTO class_masteries (class_id, object_category_id)
VALUES (1, (SELECT object_category_id FROM object_categories WHERE object_category_name = 'Leather Armor'));

-- Maîtrises pour la classe 2 (Mage)
INSERT INTO class_masteries (class_id, object_category_id)
VALUES (2, (SELECT object_category_id FROM object_categories WHERE object_category_name = 'Staff'));
```
