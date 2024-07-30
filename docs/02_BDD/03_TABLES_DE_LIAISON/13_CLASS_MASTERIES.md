# 'CLASS_MASTERIES' LIASON TABLE

```sql
CREATE TABLE class_masteries (
    class_id INT,
    object_category_id INT,
    PRIMARY KEY (class_id, object_category_id),
    FOREIGN KEY (class_id) REFERENCES classes(class_id),
    FOREIGN KEY (object_category_id) REFERENCES object_categories(object_category_id)
);
```
