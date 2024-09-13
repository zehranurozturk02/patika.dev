# patika.dev

--select * from film order by baslık ,tanım

--select*from film where uzunluk>60 and uzunluk<75

--select*from film  where kira_bedeli=0.99 and degistirme_ucreti=12.99 or degistirme_ucreti=28.99

select * from film where uzunluk<50 and kira_bedeli!=2.99 or kira_bedeli!=4.99

--                 ÖDEV 2

-- select * from film where kira_bedeli between 12.99 and 16.99

 -- select * from film where kira_bedeli in(0.99,2.99,4.99) and degistirme_ucreti in(12.99,15.99,28.99)

  --                ÖDEV 3

 --select baslık from film where baslık like '%t% ' or baslık like '%T%'

 select * from film where baslık like'C%' and uzunluk>90 and kira_bedeli=2.99
 --               ÖDEV 4

 --select distinct degistirme_ucreti from film order by degistirme_ucreti 

 --select count(distinct degistirme_ucreti) from film

 select * from film  count where (baslık like 'T%' and değerlendirme ='G') 

--                ÖDEV 5

--select top 5 * from film where baslık like'%n' order by uzunluk desc 

--2?

--            ÖDEV 6

select AVG(kira_bedeli) from film

select count( baslık ) as 'miktar' from film where baslık like'C%'

select max(uzunluk)from film where kira_bedeli =0.99

select count(distinct (degistirme_ucreti)) from film where uzunluk>150

--				ÖDEV 7 ??????????

--SELECT baslık FROM film GROUP BY değerlendirme;

--SELECT degistirme_ucreti, COUNT(*) AS film_sayısı FROM film GROUP BY degistirme_ucreti
--HAVING COUNT(*) > 50 ORDER BY film_sayısı DESC;


--ÖDEV 8

--select *from employe

--update employe set id='51' where id='1';
--update employe set id='52' where id='2';

--update employe set name='ibrahimGüncel' where name='Ibrahim';
--update employe set id='28' where name='Marlo';

--update employe set date='2024-01-01' where id='3';

--UPDATE İŞLEMİ YAPTIM 5 TANE VERİYE

--delete from employe where id='4';
--delete from employe where date='2024-07-07';
--delete from employe where email='mkerwen4@gmpg.org';
--delete from employe where name ='Karin';
--delete from employe where id='6';

--SİLME İŞLEMİ YAPTIM 5 TANE VERİYE

select *from employe

-- ÖDEV 9

--select city.name,country.name from city
--inner join country on city_id = country_id;

--select customers.first_name,customers.last_name,payment.payment_id from customers
--inner join payment on customers.musteri_id=payment.payment_id 

--select customers.first_name,customers.last_name,rental.rental_idd from customers
--inner join rental on customers.musteri_id=rental.rental_idd

-- ÖDEV 10

--select city.name,country.name from city 
--left join country on city.city_id=country.country_id

--select payment.payment_id,customers.first_name,customers.last_name from customers
--right join payment on payment_id=customers.musteri_id

--select customers.first_name,customers.last_name,rental.rental_idd from customers
--full join rental on rental_idd=customers.musteri_id

--   ÖDEV 11

--SELECT first_name FROM actor UNION 
--SELECT first_name FROM customers
--ORDER BY first_name

--SELECT first_name FROM actor except 
--SELECT first_name FROM customers
--ORDER BY first_name

--ÖDEV 12

--select count(*) from film where uzunluk> (select avg(uzunluk) from film)
--select count(*)  from film where degistirme_ucreti = (select max(degistirme_ucreti)from film)

--select baslık from film where kira_bedeli = (select MIN(kira_bedeli) from film)  AND
--degistirme_ucreti= (select MIN(degistirme_ucreti)from film) order by baslık

--select customer from payment where alışveriş_saysı= (select max(alışveriş_saysı) from payment) order by customer








