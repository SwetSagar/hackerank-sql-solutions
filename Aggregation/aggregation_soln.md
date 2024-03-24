
## Revising Aggregations - The Count Function

```

SELECT COUNT(Name) FROM CITY WHERE POPULATION > 100000;

```
## Revising Aggregations - The Sum Function

```

SELECT SUM(Population) FROM CITY WHERE District = 'California';

```

## Revising Aggregations - Averages

```

SELECT AVG(Population) FROM CITY WHERE District = 'California';

```

## Average Population

```

SELECT ROUND(AVG(Population)) FROM CITY;

```


## Japan Population

```

SELECT SUM(Population) FROM CITY WHERE countrycode = 'JPN';

```

## Population Density Difference

```

SELECT MAX(Population) - Min(Population) FROM CITY;

```


## Top Earners

```

select
  salary * months,
  count(salary * months)
from employee
group by salary * months
order by salary * months desc
limit 1;

```

## Weather Observation Station 2

```

select round(sum(lat_n),2), round(sum(long_w),2) from station;

```

## Weather Observation Station 13

```

select round(sum(lat_n), 4) from station where lat_n between 38.7880 and 137.2345;

```

## Weather Observation Station 14

```

select round(lat_n, 4)
from station
where lat_n < 137.2345
order by lat_n desc
limit 1;

```

## Weather Observation Station 15

```

select
  cast(round(long_w, 4) as Decimal(20, 4))
from station
where lat_n < 137.2345
order by lat_n desc
limit 1;

```

## Weather Observation Station 16

```

select
  cast(round(lat_n, 4) as Decimal(20, 4))
from station
where lat_n > 38.7780
order by lat_n asc
limit 1;

```

## Weather Observation Station 17

```

select round(long_w, 4)
from station
where lat_n > 38.7780
order by lat_n asc
limit 1;

```


## Weather Observation Station 18

```

SELECT
  CAST(
    (MAX(LAT_N) - MIN(LAT_N)) + (MAX(LONG_W) - MIN(LONG_W)) as decimal(10, 4)
  )
FROM STATION;

```


## Weather Observation Station 19

```

select
  CAST(
    ROUND(
      SQRT(
        POWER(max(lat_n) - min(lat_n), 2) + POWER(max(long_w) - min(long_w), 2)
      ),
      4
    ) as decimal(20, 4)
  )
from station;

```

## The Blunder

```


```

## Weather Observation Station 20

```


```