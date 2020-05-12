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
``` sql
SELECT * FROM Customers
Where City = 'Paris'

SELECT * FROM Employees
WHERE City = 'London'

-- COUNT HOW MANY EMPLOYEES IN EMPLOYEE TABLE
SELECT COUNT(EmployeeID) AS "Numer of Employees " FROM Employees

-- WHICH EMPLOYEE IS A DOCKER IN EMPLOYEE TABLE
SELECT * FROM Employees WHERE TitleOfCourtesy = 'Dr.' 

-- HOW MANY PRODUCTS ARE DISCONTINUED IN PRODUCTS TABLE

SELECT COUNT(Discontinued) AS "Number of Products discontinued"
FROM Products 
WHERE Discontinued !=0

-- FIND THE COMPANYNAME CITY COUNTRY OF REGION BC
SELECT CompanyName, City, Country,Region FROM Customers WHERE Region = 'BC' 

-- FIND THE CUSTOMERS ID OF FRENCH CUSTOMERS
SELECT CustomerID, City From Customers WHERE Country = 'France'

-- ORDER BY CLUASE TO GET TOP 100

SELECT TOP 100 CompanyName FROM Customers WHERE 

-- AND KEY WORD AS A CONDITION
SELECT ProductName, UnitPrice FROM Products WHERE CategoryID = 1 AND Discontinued = '0'

-- Distint key word is used to avoid duplication

SELECT DISTINCT c.Country 
FROM Customers c
where c.ContactTitle = 'Owner' AND c.Country LIKE '[^Denmark]E%'

-- wildcard charactors 'A%' _ refers to 

--
SELECT COUNT(*)
FROM Products p
where p.UnitPrice >0 AND p.UnitPrice>29.99

SELECT ProductName, UnitPrice FROM Products WHERE ProductName LIKE 'ch%'
-- LIKE OPERATOR
SELECT *
FROM Customers WHERE Region LIKE '_A'

-- IN OPERATOR
SELECT COUNT(*)
FROM Customers c
WHERE c.Region IN ('london','singapor')


-- between operator
SELECT * FROM EmployeeTerritories
WHERE TerritoryID BETWEEN 06800 AND 09000 

-- what are the names and products ids of the products with a unit below 5.00

SELECT p.ProductName, p.productID FROM Products p  WHERE p.UnitPrice <5.00 

-- which categories have a category name with initial begining with B or S

SELECT * FROM Categories
where CategoryName Like '[bs]%'

-- How many orders are there for EmployeeIDs 5 and 7 (total of both)
SELECT * FROM Employees
SELECT COUNT(o.EmployeeID) AS "Number of orders"
FROM Orders o
where EmployeeID in (5,7)
-- good practice

SELECT COUNT(*) AS "Number of orders"
FROM Orders o
GROUP BY EmployeeID
HAVING EmployeeID in (5,7)

-- concatenation
-- SELECT * FROM Customers

SELECT c.CompanyName AS "Company Name", c.City + ', ' + c.Country 'City'
FROM Customers c

--- concatenate first and last name from employee table 

SELECT c.FirstName + ' ' + c.LastName AS "Employee name"  
FROM Employees c

-- is NULL or is NOT null
SELECT Region, c.CompanyName AS "Company Name", c.City + ', ' + c.Country 'City'
FROM Customers c where Region is null 

--- select statement to list the six counties that have region codes in the customers table
SELECT DISTINCT c.Country
FROM Customers c
where c.Region is null 
```



