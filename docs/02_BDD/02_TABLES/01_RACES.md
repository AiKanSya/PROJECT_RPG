# 'RACES' TABLE

```sql
CREATE TABLE races (
    race_id INT AUTO_INCREMENT PRIMARY KEY,
    race_name VARCHAR(255) NOT NULL,
    description TEXT,
    playable BOOLEAN NOT NULL DEFAULT FALSE,
    specific_size VARCHAR(255),
    speed DECIMAL(5, 1),
    min_age INT,
    max_age INT
);
```
