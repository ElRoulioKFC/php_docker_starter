to launch the containers : 
docker compose up

to start working with database : 

# Connection to the MySQL container
docker exec -ti php_docker_starter-mysql-1 bash

# Connect to MySQL server
mysql -uroot -psuper-secret-password

# We go to the database created when the container is launched
use my-wonderful-website;

# Creation of a "Persons" Table, with a few columns
CREATE TABLE Persons (PersonID int, LastName varchar(255), FirstName varchar(255), Address varchar(255), City varchar(255));

# Insert some data into this table
INSERT INTO Persons VALUES (1, 'John', 'Doe', '51 Birchpond St.', 'New York');
INSERT INTO Persons VALUES (2, 'Jack', 'Smith', '24 Stuck St.', 'Los Angeles');
INSERT INTO Persons VALUES (3, 'Michele', 'Sparrow', '23 Lawyer St.', 'San Diego');