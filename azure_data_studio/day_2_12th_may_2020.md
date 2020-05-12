# stand up
## attendance lateness
- Trello board update
- lesson:
- Normalisation
- task:
``` bash
Create 2 table with 


``` 
``` SQL

-- CREATING YOUR OWN DATA-BASE
CREATE DATABASE shah_khan_db

-- USING SPECIFIC DATA-BASE
USE shah_khan_db

-- CREATING A TABLE CALLED film_t
CREATE TABLE film_t
(
    
    film_id INT IDENTITY(1,1),
    film_name VARCHAR(20) NOT NULL,
    film_type VARCHAR(10),
    date_of_release DATETIME,
    director_name VARCHAR(10),
    writer_name VARCHAR(10),
    star_cast VARCHAR(10),
    film_language VARCHAR(10),
    official_website VARCHAR(30),
    plot_summary VARCHAR(max),
    film_rating INT DEFAULT 5

    PRIMARY KEY(film_id)
);
-- INSERING VALUES INTO THE TABLE
INSERT INTO film_t
(
    film_name,film_type, plot_summary  

)
VALUES
(
    'speed', 'sharkA', 'TICIANIC'
)
SELECT * FROM film_t WHERE film_rating IS NULL
-- ALTER TABLE film_t ADD film_rating INT

-- SELECT ALL DATA FROM TABLE CALLED fiml_t
SELECT * FROM film_t

-- ALTER OPTIONS
ALTER TABLE film_tab ADD lead_hero VARCHAR(10);
ALTER TABLE flim_tab DROP COLUMN plot_summary;  

-- SP HELP TO VIEW IF THE TABLE IS CREATED
SP_HELP film_t

-- -- SP_HELP film_tab

-- DROP OPTIONS FOR TABLE COLUMN ETC.

-- -- DROP TABLE film_table

DROP TABLE film_t
-- DROP TABLE WILL DELETE THE TABLE FROM THE DATA-BASE

ALTER TABLE film_tab

-- update statement with set and where condition
UPDATE film_t
SET film_rating = 10
WHERE film_rating=5

-- delete statement
DELETE FROM film_t WHERE film_name='sharkA'


-- ON DELETE CASCADE 
```


