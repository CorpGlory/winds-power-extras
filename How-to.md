- (optional) Create database
```SQL
CREATE DATABASE winds;
```
- Connect to database
```SQL
\connect winds;
```
- Create table
```SQL
CREATE TABLE wind_pwr_spd(
  time TIMESTAMP NOT NULL PRIMARY KEY,
  speed NUMERIC,
  power NUMERIC
);
```
- Insert data

Full insert command set to import [dataset.csv](dataset.csv) can be found in [insert.sql](insert.sql)

Example:
```SQL
INSERT INTO wind_pwr_spd(time, power, speed) VALUES (NOW(), 3055.86957961, 25);
```


