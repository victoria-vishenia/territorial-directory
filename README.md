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


**Tools**

The application is developed using Java Collections API, Java Stream API, Hibernate, MySQL, Redis, Docker.

**User instruction**
 
To configurate Session Factory for MySQL let's set up method prepareRelationalDb() in Main.Class. 
To configurate RedisClient use prepareRedisClient() method in Main.Class.
To create schema in MySQL, import CityCountry.sql dump file.
For set up MySQL and Redis you can use Docker.
After starting the project, you could compare efficency of MySQL queries and commands in Redis.
