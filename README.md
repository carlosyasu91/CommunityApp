# BookShareApp

Users
Books
UserBooks
BookRequest

This is a SQL starter guide for Users who want to start learning about SQL and getting comfortable with SQL queries.

### Topics

1. Create tables
2. SELECT
3. CROSS JOIN
4. INNER JOIN


## Creating Tables



### First Schema



### Last Iteration

CREATE TABLE Users(
  id INT NOT NULL AUTO_INCREMENT,
  username VARCHAR(255),
  email VARCHAR(255),
  type INT
  PRIMARY KEY (id)
);

CREATE TABLE UserTypes(
  id INT NOT NULL AUTO_INCREMENT,
  type VARCHAR(255),
  PRIMARY KEY (id)
);

CREATE TABLE Books(
  id INT NOT NULL AUTO_INCREMENT,
  title VARCHAR(255),
  author VARCHAR(255),
  description VARCHAR(255),
  category VARCHAR(255),
  PRIMARY KEY (id)
);

CREATE TABLE User_Books(
  id INT NOT NULL AUTO_INCREMENT,
  UserID INT FOREIGN KEY REFERENCES Users(id),
  BookID INT FOREIGN KEY REFERENCES Books(id),
  PRIMARY KEY (id)
);

CREATE TABLE Friends(
  id INT NOT NULL AUTO_INCREMENT,

);

INSERT INTO Users (username, email) VALUES ('John', 'john33@john.com');
INSERT INTO Users (username, email) VALUES ('Bradley', 'bradley@gmail.com');
INSERT INTO Users (username, email) VALUES ('Dominic', 'dom@gmail.com');
INSERT INTO Users (username, email) VALUES ('Clint', 'clint@gmail.com');
INSERT INTO Users (username, email) VALUES ('Elizabeth', 'daniel@daniel.com');

INSERT INTO UserTypes (type)

INSERT INTO Books (title, author, description, category) 
VALUES ('The Lord of the Rings','J. R. R. Tolkien', 'Presents the epic depicting the Great War of the Ring', 'Fiction');
INSERT INTO Books (title, author, description, category) 
VALUES ('Mindset', 'Carol Dweck' , 'World-renowned Stanford University psychologist Carol Dweck, in decades of research on achievement and success, has discovered a truly groundbreaking idea—the power of our mindset.');
INSERT INTO Books (title, description, category) 
VALUES ('How To Win Friends and Influence People', 'Dale Carnegie' , 'You can go after the job you want...and get it! You can take the job you have...and improve it!');

INSERT INTO User_Books VALUES ()

1. SELECT * FROM Users;

2. SELECT * FROM Users ORDER BY email;

3. SELECT COUNT(*) FROM Users;

4. SELECT * FROM Users CROSS JOIN Books;

2. SELECT username, email from Users;

