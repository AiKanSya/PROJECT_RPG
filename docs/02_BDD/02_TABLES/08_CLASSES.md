# 'CLASSES' TABLE

```sql
CREATE TABLE classes (
    class_id INT AUTO_INCREMENT PRIMARY KEY,
    class_name VARCHAR(50) NOT NULL,
    description TEXT,
    playable BOOLEAN NOT NULL DEFAULT FALSE -- Indique si la classe est jouable ou non
);
```
