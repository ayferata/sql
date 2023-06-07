# sql
Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması?
SELECT AVG(rental_rate) FROM film;
SELECT ROUND(AVG(rental_rate),3) FROM film;

Film tablosunda bulunan filmlerden kaç tanesi 'D' karakteri ile başlar?

SELECT COUNT(*) FROM film
WHERE title LIKE 'D%';

Film tablosunda bulunan filmlerden rental_rate değeri 4.99 a eşit olan en uzun (length) film kaç dakikadır?

SELECT MAX(length) FROM film
WHERE rental_rate = 4.99;

Film tablosunda bulunan filmlerin uzunluğu 100 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?


SELECT COUNT(DISTINCT replacement_cost) FROM film
WHERE length >100;
