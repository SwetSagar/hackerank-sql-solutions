# Hackerrank Solution to SQL Part 1 Basic Select

## Basic Select

### Revising the Select Query

```
select * from CITY where CountryCode = "USA" and POPULATION > 100000;
```

### Revising the Select Query II

```

select NAME from CITY where POPULATION > 120000 and CountryCode = "USA";

```

### Select All

```
select * from CITY;

```

### Select By ID

```

select * from CITY where ID = "1661";

```

### Japanese Cities' Attributes

```

select * from CITY where COUNTRYCODE = "JPN";

```

### Japanese Cities' Names

```

select NAME from CITY where COUNTRYCODE = "JPN";

```

### Weather Observation Station 1

```

select city, state from STATION;

```

### Weather Observation Station 3

```

select distinct CITY from STATION where ID%2 = 0;

```

### Weather Observation Station 4

```
select COUNT(CITY) - COUNT(DISTINCT CITY) FROM STATION;

```

### Weather Observation Station 5

```

select city, length(city) from station order by length(city) desc, city asc limit 1;

```

### Weather Observation Station 6

```

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[aeiou]';

```

### Weather Observation Station 7

```

SELECT DISTINCT CITY FROM STATION WHERE CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u';

```

### Weather Observation Station 8

```

SELECT DISTINCT city FROM station WHERE city REGEXP '^[aeiou].*[aeiou]$'

```

### Weather Observation Station 9

```

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[^aeiou]';

```

### Weather Observation Station 10

```

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '[^aeiou]$';

```

### Weather Observation Station 11

```

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[^aeiouAEIOU].*' OR CITY REGEXP '[^aeiouAEIOU]$';

```

### Weather Observation Station 12

```

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[^aeiou]' AND CITY REGEXP '[^aeiou]$'; 

```

### Higher Than 75 Marks

```

SELECT NAME 
FROM STUDENTS
WHERE Marks > 75 
ORDER BY RIGHT(Name,3),ID ASC;

```

### Employee Names

```

SELECT NAME FROM Employee ORDER BY NAME ASC; 

```

### Employee Salaries

```

SELECT name FROM Employee WHERE salary > 2000 AND months < 10 ORDER BY employee_id ASC;

```
