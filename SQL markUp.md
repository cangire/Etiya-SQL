INNER JOIN

select * from addresses a INNER JOIN cities c on c.id = a.city_id

![inner-join.PNG](https://www.dropbox.com/s/d5wv7aq99svzulg/inner-join.PNG?dl=0&raw=1)

OUTER JOIN

select * from addresses a full outer JOIN cities c on c.id = a.city_id

![full-outer-join.PNG](https://www.dropbox.com/s/v6di19iw5imb7wm/full-outer-join.PNG?dl=0&raw=1)

LEFT JOIN

select* from product_categories pc left join products ON products.id = pc.product_id

![left join.PNG](https://www.dropbox.com/s/lm12075hgu8sa4j/left%20join.PNG?dl=0&raw=1)

RIGHT JOIN

select* from addresses a RIGHT join customers ON customers.id = a.customer_id

![right join.PNG](https://www.dropbox.com/s/8kki0kzm83ckuca/right%20join.PNG?dl=0&raw=1)

BEFORE INSERT

![before insert.PNG](https://www.dropbox.com/s/m8jija1qbqblq0t/before%20insert.PNG?dl=0&raw=1)

INSERT

INSERT INTO categories(name)
values('Home staff')

![after insert.PNG](https://www.dropbox.com/s/1agbzdqfop412x8/after%20insert.PNG?dl=0&raw=1)

UPDATE

UPDATE categories set name='Toys' where name='Home staff'
select * from categories

![uppp.PNG](https://www.dropbox.com/s/04gse53dkvl8fqm/uppp.PNG?dl=0&raw=1)

IN

select * from categories ca where ca.name IN

![IN.PNG](https://www.dropbox.com/s/2efoqocph0a5tex/IN.PNG?dl=0&raw=1)

BETWEEN

select stock from products p where p.stock between 30 and 150

![between.PNG](https://www.dropbox.com/s/l9j3c3b9k8ccqcu/between.PNG?dl=0&raw=1)

GROUP BY

select count(p.name) as "product count",pc.category_id 
from product_categories pc 
Inner join products p on pc.product_id=p.id
group by pc.category_id

![group by.PNG](https://www.dropbox.com/s/ss3z8ptddec43kg/group%20by.PNG?dl=0&raw=1)