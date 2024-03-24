# Advance Select

## Type of Triangle

```
select
  (
    case
      when A + B <= c
      or A + C <= B
      or B + C <= A then 'Not A Triangle'
      when A = B
      and A = C
      and B = C then 'Equilateral'
      when A = B
      or A = C
      or B = C then 'Isosceles'
      when A != B
      and A != c
      and B != c then 'Scalene'
    end
  )
from TRIANGLES;

```


## The PADS


```

select
  CONCAT(name, '(', left (occupation, 1), ')')
from occupations
order by name asc;

```

## Occupations 

```

```

### Binary Tree Nodes

```

```

### New Companies

```

```