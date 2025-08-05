# goit-rdb-hw-03

## Task 1
```
-- 1.1
select * from mydb.products;

-- 1.2
select name, phone from mydb.shippers;
```

## Task 2
```
select avg(price) as avg_price, max(price) as max_price, min(price) as min_price
from mydb.products;
```

## Task 3
```
select distinct category_id, price
from mydb.products
order by price desc
limit 10;
```

## Task 4
```
select count(*)
from mydb.products
where price >= 20 and price <= 100;
```

## Task 5
```
select supplier_id, count(id) as products_count, avg(price) as avg_price
from mydb.products
group by supplier_id;
```
