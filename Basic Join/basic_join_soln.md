# Basic Joins


## The Report



## Population Census

```
select sum(city.population) from city 
join country on city.countrycode = country.code
where country.continent = 'Asia';

```

##  African Cities

```
select city.name from city 
left join country on city.countrycode = country.code where country.continent = 'Africa';

```

## Average Populaiton of Each  Continent

```

```

## Average Population of Each Continent

```
select country.continent, FLOOR(avg(city.population)) from city join country on city.countrycode = country.code group by continent;  

```

## Top Competitors 

```
```

## Ollivander's Inventory

```
```

## Challenges

```

```

## Contest Leaderboard

```

```