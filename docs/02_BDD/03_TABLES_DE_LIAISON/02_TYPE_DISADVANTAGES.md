# 'TYPE_DISADVANTAGES' LIASON TABLE

```sql
CREATE TABLE type_disadvantages (
    type_id INT,
    element_id INT,
    PRIMARY KEY (type_id, element_id),
    FOREIGN KEY (type_id) REFERENCES types(type_id),
    FOREIGN KEY (element_id) REFERENCES elements(element_id)
);
```
