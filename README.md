Install PostgreSQL on your machine following. the instructions:
	=>  Postgres 12.10 was installed.
	      Used all default settings!
 
 Connect to the DB server by terminal Practice whatever we did in the class:
	=> a. Used psql shell.
	     b. Start the shell, press enter till the option for password is displayed. Used password. ( while putting the password, you can’t see the input or any character.) 
	     c.  After connecting, you can create a database by using the following command..
                       CREATE DATABASE b2201; 
                      CREATE DATABASE
	     d.  Now create a table in the database
	          
CREATE TABLE info_table
CREATE TABLE Info_Table (
b2201(# ID BIGSERIAL NOT NULL PRIMARY KEY,
b2201(# First_Name VARCHAR(200) NOT NULL,
b2201(# Last_Name VARCHAR(200) NOT NULL,
b2201(# Address VARCHAR(100) NOT NULL ); 
CREATE TABLE


INSERT INTO info_table
b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('001', 'Jamal', 'Azad', 'New York');                                                                                                   
INSERT 0 1                                                                                                                                                                                                         b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('002', 'Jalal', 'Ahmed', 'New Jersy');                                                                                                 
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('003', 'Md', 'Islam', 'Dhaka');                                                                                                        
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('004', 'Salehuddin', 'Talukder', 'Sylhet');                                                                                            
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('005', 'Aminur', 'Rasul', 'Comilla');                                                                                                  
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('006', 'Rubel', 'Salam', 'Sylhet');                                                                                                    
INSERT 0 1                                                                                                                                                                                                          b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('007', 'Noshin', 'Rahman', 'Jessore');                                                                                                 
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('008', 'Mara', 'Lagapa', 'New York');                                                                                           
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('009', 'Taha', 'Khan', 'Moulvibazar');                                                                                                 
INSERT 0 1                                                                                                                                                                                                           b2201=# INSERT INTO info_table (Id, First_name, Last_name, Address) VALUES ('010', 'Amin', 'Khan', 'Barisal');                                                                                                     
INSERT 0 1    
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  

SELECT From info_table
b2201=# SELECT * FROM info_table;                                                                                                                                                                                   id | first_name | last_name |   address                                                                                                                                                                           ----+------------+-----------+-------------                                                                                                                                                                          1 | Jamal      | Azad      | New York                                                                                                                                                                              2 | Jalal      | Ahmed     | New Jersy                                                                                                                                                                             3 | Md         | Islam     | Dhaka                                                                                                                                                                                 4 | Salehuddin | Talukder  | Sylhet                                                                                                                                                                                5 | Aminur     | Rasul     | Comilla                                                                                                                                                                               6 | Rubel      | Salam     | Sylhet                                                                                                                                                                                7 | Noshin     | Rahman    | Jessore                                                                                                                                                                               8 | Mara       | Lagapa    | New York                                                                                                                                                                              9 | Taha       | Khan      | Moulvibazar                                                                                                                                                                          10 | Amin       | Khan      | Barisal                                                                                                                                                                             (10 rows)                                                                                                                                                                                                                    




UPDATE info_table
b2201=# UPDATE info_table SET Address= 'New Jersey' WHERE id= 2;
UPDATE 1

b2201=# SELECT * FROM info_table;
 id | first_name | last_name |   address
----+------------+-----------+-------------
  1 | Jamal      | Azad      | New York
  3 | Md         | Islam     | Dhaka
  4 | Salehuddin | Talukder  | Sylhet
  5 | Aminur     | Rasul     | Comilla
  6 | Rubel      | Salam     | Sylhet
  7 | Noshin     | Rahman    | Jessore
  8 | Mara       | Lagapa    | New York
  9 | Taha       | Khan      | Moulvibazar
 10 | Amin       | Khan      | Barisal
  2 | Jalal      | Ahmed     | New Jersey
(10 rows)


SELECT ORDER BY id
b2201=# SELECT * FROM info_table ORDER BY id;
 id | first_name | last_name |   address
----+------------+-----------+-------------
  1 | Jamal      | Azad      | New York
  2 | Jalal      | Ahmed     | New Jersey
  3 | Md         | Islam     | Dhaka
  4 | Salehuddin | Talukder  | Sylhet
  5 | Aminur     | Rasul     | Comilla
  6 | Rubel      | Salam     | Sylhet
  7 | Noshin     | Rahman    | Jessore
  8 | Mara       | Lagapa    | New York
  9 | Taha       | Khan      | Moulvibazar
 10 | Amin       | Khan      | Barisal
(10 rows)

DELETE from info_table
b2201=# DELETE FROM info_table WHERE id='10';
DELETE 1
b2201=# SELECT * FROM info_table;
 id | first_name | last_name |   address
----+------------+-----------+-------------
  1 | Jamal      | Azad      | New York
  3 | Md         | Islam     | Dhaka
  4 | Salehuddin | Talukder  | Sylhet
  5 | Aminur     | Rasul     | Comilla
  6 | Rubel      | Salam     | Sylhet
  7 | Noshin     | Rahman    | Jessore
  8 | Mara       | Lagapa    | New York
  9 | Taha       | Khan      | Moulvibazar
  2 | Jalal      | Ahmed     | New Jersey
(9 rows)

Installed PGAdmin 4 and worked on it.
Practice SQL queries that I have learned on PGAdmin 4.
Screenshot 


 

Import a sample database using this instruction from
LinkOne: https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/ 
LinkTwo:
https://www.postgresqltutorial.com/postgresql-getting-started/load-postgresql-sample-database/












Open pgAdmin and create a new database named ‘dvdrental’


Restore dvdrental database from computer


After uploading the database







Data on the files……..



C. Practice to update data on the database.

