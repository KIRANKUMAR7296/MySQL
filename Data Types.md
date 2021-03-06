# Data Types

```mysql
# Numeric: Integer 
INT 
INTEGER 
# e.g. 47, 500, 235454345535

# Numeric: Fixed Point  
DECIMAL(Precision, Scale) 
DECIMAL(1, 2)
DECIMAL(8, 3)
DECIMAL(10, 0)
# e.g. 3.47, 10000000.474, 1234567890

# Numeric: Floating Point
# Never use FLOAT for money.
NUMERIC(1, 2)
NUMERIC(9, 2)
FLOAT
DOUBLE
# e.g. 3.47, 1234567.89
```

```mysql
# String - Fixed Length 
# Fixed length strings are prefixed or padded with 0's
CHAR(length)
'2286700', '4A11781', 'MB 4554'

# String: Variable Length 
VARCHAR(length)
'Kirankumar Yadav', 'Ram Kapoor', 'Chinaswami Mutuswami Krishnagopal Santhnam'

# Binary Strings: Non text based strings.
BINARY(length) 
VARBINARY(length)

# BLOB & TEXT: Binary Large Object Storage
# Stores images, audios and other binary objects.

# BLOB:
TINYBLOB
BLOB
MEDIUMBLOB
LONGBLOB

# TEXT:
TINYTEXT
TEXT
MEDIUMTEXT
LONGTEXT
```

````mysql
# Date and Time
# Current Date and Time ( Format: yyyy-mm-dd hh:mm:ss )
SELECT NOW(); 
DATE 
DATETIME  : 2022-02-07 21:45:55
TIMESTAMP : 1996-01-01 to 2022-01-01

DROP TABLE IF EXISTS Temp;

CREATE TABLE Temp (
  ID INT UNSIGNED UNIQUE AUTO_INCREMENT PRIMARY KEY,
  Stamp DATETIME DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
  Name VARCHAR(64)
);

INSERT INTO Temp (Name)
VALUES ('Kirankumar Yadav')
````

```mysql
# Enumerations
ENUM: Single value from list
SET: Multiple values from list


# Specialty
```

### Arithmetic Operators:

```mysql
SELECT 4 + 5;
SELECT 7 - 5;
SELECT 7 / 5;
SELECT 7 DIV 5;
SELECT 7 % 5;
SELECT 7 MOD 5;
```
