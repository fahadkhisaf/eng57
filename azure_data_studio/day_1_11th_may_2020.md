# Day 1 - 11th May 2020
## Introduction to database
### Objectives

- understand database terminology
- What data base do we use in everyday life?
```markdown
mobile phone 
hard drive
github
```
```
Tables:
 
column are vertical and rows are horizontal
columns are attributes

<<<<<<< HEAD
```
```
database/ tabels relationships:
- one to one  
- one to many
- many to many
```
Primary key must be unique
- Normalisation
- setting up docker with vm for Saskia
-
=======
``` 
``` sql

CREATE DATABASE shah_khan_db add
USE shah_khan_db

CREATE TABLE film_tab
(
    film_id INT IDENTITY(1,1),
    film_name VARCHAR(20),
    film_type VARCHAR(10),
    date_of_release DATETIME,
    director_name VARCHAR(10),
    writer_name VARCHAR(10),
    star_cast VARCHAR(10),
    film_language VARCHAR(10),
    official_website VARCHAR(30),
    plot_summary VARCHAR(max)



);

INSERT INTO film_tab
(
    film_name,film_type, plot_summary


)
VALUES
(
    'Geo-Storm', 'sci-fi', 'maximum'
)

SELECT * FROM film_tab
-- ALTER TABLE film_tab ADD lead_hero VARCHAR(10);
-- -- ALTER TABLE flim_tab DROP COLUMN plot_summary;  
-- SP_HELP film_tab

-- -- SP_HELP film_tab
-- -- DROP TABLE film_table
-- DROP TABLE film_tab

-- ALTER TABLE film_tab
```
- Normalisation
### To be cont
>>>>>>> 49015725dd37c2f2f3328d849f0c16681eaadf6b
