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













