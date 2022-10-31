### [SQLzoo](https://sqlzoo.net/wiki/SQL_Tutorial) tutorial Solutions ###
1.[SELECT BASICS](#basics)\
2.[SELECT NAME](#name)\
3.[SELECT from World](#World)\
4.[SELECT from Nobel](#nobel)\
5.[SELECT within SELECT](#select)\
6.[SUM and COUNT](#sum)\
7.[JOIN](#join)\
8.[More JOIN operations](#morejoin)\
9.[Using Null](#null)\
10.[Numeric Examples](#numeric)\
11.[Window function](#window)\
12.[COVID 19](#covid)\
13.[Self join](#selfjoin)\
14.[Tutorial Quizzes](#quizes)\


#### SELECT BASICS <a name="basics"></a> ####

1.Modify it to show the population of Germany
 ```
 SELECT population FROM world
  WHERE name = 'Germany';
 
 ```
2.Show the name and the population for 'Sweden', 'Norway' and 'Denmark'.
 ```
SELECT name, population FROM world
  WHERE name IN ('Sweden', 'Norway', 'Denmark');
 
 ```

3. Which countries are not too small and not too big?
 ```
SELECT name, area FROM world
  WHERE area BETWEEN 200000 AND 250000;
 
 ```
#### SELECT NAME <a name="name"></a> ####

1.Find the country that start with Y
 ```
SELECT name FROM world
  WHERE name LIKE 'Y%';
 
 ```
2.Find the countries that end with y
 ```
SELECT name FROM world
  WHERE name LIKE '%Y';
 
 ```
 3.Find the countries that contain the letter x
 ```
SELECT name FROM world
  WHERE name LIKE '%x%';
 
 ```
 4.Find the countries that end with land
  ```
SELECT name FROM world
  WHERE name LIKE '%land';
 
 ```
 5.Find the countries that start with C and end with ia
  ```
SELECT name FROM world
  WHERE name LIKE 'C%' AND name LIKE '%IA';
 
 ```
 6.Find the country that has oo in the name
   ```
SELECT name FROM world
  WHERE name LIKE '%oo%'
 
 ```
 7.Find the countries that have three or more a in the name
 ```
 SELECT name FROM world
  WHERE name LIKE '%a%a%a%';
  ```
 8.Find the countries that have "t" as the second character.
 ```
 SELECT name FROM world
 WHERE name LIKE '_t%'
ORDER BY name;
 ```
 9.Find the countries that have two "o" characters separated by two others.
 ```
 SELECT name FROM world
 WHERE name LIKE '%o__o%';
 ```
 10.Find the countries that have exactly four characters.
 ```
 SELECT name FROM world
 WHERE name LIKE '____'
 ```
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 

