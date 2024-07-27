CREATE TABLE equipment (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name VARCHAR NOT NULL,
    category VARCHAR NOT NULL,
    price FLOAT NOT NULL,
    available BOOLEAN DEFAULT TRUE
);

## Table: equipment

| Column    | Type    | Constraints                |
|-----------|---------|----------------------------|
| id        | INTEGER | PRIMARY KEY AUTOINCREMENT  |
| name      | VARCHAR | NOT NULL                   |
| category  | VARCHAR | NOT NULL                   |
| price     | FLOAT   | NOT NULL                   |
| available | BOOLEAN | DEFAULT TRUE               |

This table stores information about the film equipment available for rent.