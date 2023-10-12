# Territorial directory

**Description**

Application for obtaining data from the territorial directory. Data is stored in MySQL and Redis. Compares the speed of retrieving the same data from MySQL and Redis.
My results: 
1) Redis:	170 ms
MySQL:	152 ms

2) Redis:	161 ms
MySQL:	152 ms

3) Redis:	241 ms
MySQL:	158 ms

And results after adding P6Spy:

1) Redis:	179 ms
MySQL: 222 ms

2) Redis:	140 ms
MySQL:	132 ms

3) Redis:	116 ms
MySQL:	133 ms

**Tools**

The application is developed using Java Collections API, Java Stream API, Hibernate, MySQL, P6Spy, Redis, Docker.

**User instruction**
 
To configurate Session Factory for MySQL let's set up method prepareRelationalDb() in Main.Class. 
To configurate RedisClient use prepareRedisClient() method in Main.Class.
In lines LOGIN and PASSWORD i used stubs. There should be relevant values for connection to your MySQL.
To create schema in MySQL, import CityCountry.sql dump file.
For set up MySQL and Redis you can use Docker.
After starting the project, you could compare efficency of MySQL queries and commands in Redis.
