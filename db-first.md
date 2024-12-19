# DB-FIRST

Consegna: Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

| name                  | type         | attributes                          | key     | note                                                                 |
| --------------------- | ------------ | ----------------------------------- | ------- | -------------------------------------------------------------------- |
| id                    | BIGINT(20)   | NOT NULL - AUTOINCREMENT - UNSIGNED | PRIMARY |                                                                      |
| brand                 | VARCHAR(20)  | NOT NULL                            |         |                                                                      |
| model                 | VARCHAR(40)  | NOT NULL                            |         |                                                                      |
| matriculation_at      | DATE         | NOT NULL                            |         |                                                                      |
| number_previous_owner | TINYINT      | NOT NULL - DEFAULT(1)               |         |                                                                      |
| color                 | VARCHAR(20)  | NOT NULL                            |         |                                                                      |
| body_type             | VARCHAR(20)  | NOT NULL                            |         |                                                                      |
| conditions            | VARCHAR(20)  | NOT NULL                            |         |                                                                      |
| mileage               | INT          | NOT NULL                            |         |                                                                      |
| price                 | DOUBLE(10,2) | NOT NULL                            |         |                                                                      |
| car_plate             | CHAR(7)      | NOT NULL                            |         |                                                                      |
| VIN                   | CHAR(17)     | NOT NULL                            |         |                                                                      |
| power_type            | CHAR(1)      | NOT NULL                            |         | "1": gasoline, "2": diesel, "3": electric, "4": hybrid, "5": methane |
| traction              | CHAR(1)      | NOT NULL - DEFAULT(1)               |         | "1": FWD, "2": RWD, "3": AWD                                         |
| engine_horsepower     | VARCHAR(4)   | NOT NULL                            |         |                                                                      |
| engine_model          | VARCHAR(20)  | NOT NULL                            |         |                                                                      |
| other_info            | TEXT         | NULL                                |         | Allestimento, elenco optional, altro                                 |
