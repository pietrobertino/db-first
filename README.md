Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.


DATABASE CONCESSIONARIO

## Table name: cars

## Columns:

- id PRIMARY KEY (INT UNIQUE NOTNULL AUTO_INCREMENT)         INDEX
- car_plate (CHAR(7) UNIQUE NOTNULL)
- car_model (VARCHAR(15) NOTNULL)                              INDEX
- car_manufacturer (VARCHAR(15) NOTNULL)                     INDEX
- production_year (YEAR NOTNULL)
- fuel_type (VARCHAR(10) NOTNULL)
- color (VARCHAR(15) NULL)
- generation (TINYINT NULL)
- seat_number (TINYINT NULL)
- door_number (TINYINT NULL)
- vehicle_condition (VARCHAR(50) NOTNULL)
- price (DECIMAL(8,2) NOT NULL)  
- mileage (SMALLINT NOTNULL)
- number_of_previous_owners (TINYINT DEFAULT(1))
- features (VARCHAR(255) NULL)
- notes (TEXT NULL)