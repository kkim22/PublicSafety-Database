# Public Safety Database Project

## Description
It is an imitation of a database program which a college public safety offices use to manage data relating to cars, parking permits, tickets, and people data. This project has taught me how to construct a reliable database where the users can easily create, read, update, delete and search relevant data. Also, I learned the core concepts of building database and proper ways of connecting tables using primary key and foreign key.

-Features include
1. When user is inserting into People table, depending either faculty or staff, user can add extra data.
	* Extra Data: 
	* Student table has three attributes(Person_ID, class, dorm_name)
	* Faculty table has two attributes(Person_ID, department_name)
2. If person who is registering a car at school is different than person who registered the car at DMV, user can add extra data
	* Extra Data: 
	* dmv_owner table has three attributes(first_name, last_name, Person_ID)
3. People table has 7 attributes (first_name, last_name, Person_ID, email, driver_license_num, home_address, current_address)
4. Car table has 4 attributes(License_plate_num, registration_number,color, model)
5. Permit has 4 attributes(Person_ID, License_plate_num, Permit_num, type)
6. User can delete data from People or Car table even if data from Permit table is related to it. It asks user if one wants to erase the permit also
7. When user wants to delete or update from People table, Car table, or Permit table user can type Person_ID/persons name, License_plate_num/model, or Permit_num according to which table they choose
8. User can search People table by typing person's Person_ID or person's name, and from Car table by typing car's License_plate_num, or model

## How to Run
1. Clone github repository to local computer

2. Install 
- **ruby 2.2.1p85** (2015-02-26 revision 49769)
- **SQLite** (version 3.8.2 2013-12-06)
- **Gem Highline**
- **Gem Minitest**

3. From command line, 

type: "ruby main.rb" to run the application

-When you log in, you need I.D. and password. (ID: 1234 Password: 1234)

-You can check the data type of the attributes in data.sql file

type: "ruby test.rb"  to run the function tests

type: "ruby crud_test.rb" to run the create, read, update, and delete tests
