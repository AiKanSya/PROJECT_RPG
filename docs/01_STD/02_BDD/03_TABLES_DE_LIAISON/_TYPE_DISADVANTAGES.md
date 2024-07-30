# 'TYPE_DISADVANTAGES' LIASON TABLE

## STRUCTURE DE TABLE

```sql
CREATE TABLE type_disadvantages (
    type_id INT,
    element_id INT,
    PRIMARY KEY (type_id, element_id),
    FOREIGN KEY (type_id) REFERENCES types(type_id),
    FOREIGN KEY (element_id) REFERENCES elements(element_id)
);
```

## EXEMPLE D'INSERTION DE DONNEES

```sql
INSERT INTO type_disadvantages (type_id, element_id) VALUES (2, 1); -- Mort-vivant a un désavantage face à Sacré
INSERT INTO type_disadvantages (type_id, element_id) VALUES (2, 2); -- Mort-vivant a un désavantage face à Feu
INSERT INTO type_disadvantages (type_id, element_id) VALUES (1, 3); -- Humanoide a un désavantage face à Eau (exemple)
```
