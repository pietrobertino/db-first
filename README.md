Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.


DATABASE CONCESSIONARIO

## Table name: cars

## Columns:

- id PRIMARY KEY (INT UNIQUE NOTNULL AUTO_INCREMENT)         INDEX
- targa (CHAR(7) UNIQUE NOTNULL)
- modello (VARCHAR(15) NOTNULL)                              INDEX
- casa produttrice (VARCHAR(15) NOTNULL)                     INDEX
- anno (YEAR NOTNULL)
- alimentazione (VARCHAR(10) NOTNULL)
- colore (VARCHAR(15) NULL)
- generazione (TINYINT NULL)
- numero di posti (TINYINT NULL)
- numero di porte (TINYINT NULL)
- condizioni (VARCHAR(50) NOTNULL)
- prezzo (DECIMAL(8,2) NOT NULL)  
- kilometri di usura (SMALLINT NOTNULL)
- numero di proprietari precedenti (TINYINT DEFAULT(1))
- features (VARCHAR(255) NULL)
- note (TEXT NULL)