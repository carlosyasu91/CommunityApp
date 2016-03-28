# CommunityApp

This is a SQL starter guide for people who want to start learning about SQL and getting comfortable with SQL queries.

### Topics

1. Create tables
2. SELECT
3. CROSS JOIN
4. INNER JOIN
5. 


## Creating Tables



### First Schema



### Last Iteration

CREATE TABLE People(
  id INT NOT NULL AUTO_INCREMENT,
  firstName VARCHAR(255),
  lastName VARCHAR(255),
  age INT
  PRIMARY KEY (id)
);

INSERT INTO People (firstName, lastName, age) VALUES ('John', 'Snow', 25);
INSERT INTO People (firstName, lastName, age) VALUES ('Bradley', 'Gill', 43);
INSERT INTO People (firstName, lastName, age) VALUES ('Dominic', 'Hanson', 18);
INSERT INTO People (firstName, lastName, age) VALUES ('Clint', 'Lawrence', 40);
INSERT INTO People (firstName, lastName, age) VALUES ('Elizabeth', 'Daniel', 29);

CREATE TABLE Pets(
  id INT NOT NULL AUTO_INCREMENT
  type INT ,
  name VARCHAR(255),
  owner VARCHAR(255),
);

CREATE TABLE Jobs(
  id INT,
  jobTitle VARCHAR(255),
  hoursPerWeek VARCHAR(255)
);

CREATE TABLE Friends(
  id INT,
  userId INT,
  frienId INT
);


1. SELECT * FROM People;

2. SELECT * FROM People ORDER BY age;

3. SELECT * FROM People ORDER BY age DESC;



2. SELECT firstName, lastName from People;

