# -ODEV4-SQL
dvdrental sorgu senaryoları çözümleri
Sorgu 1- film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
Çözüm 1-SELECT DISTINCT replacement_cost FROM film;
<img width="524" alt="Ekran Resmi 2023-03-01 23 43 33" src="https://user-images.githubusercontent.com/116847744/222260657-a5a2b2f6-90ba-48f1-a344-f5d5ea4926a1.png">

Sorgu 2- film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
Çözüm 2-SELECT COUNT(DISTINCT replacement_cost) FROM film;
<img width="531" alt="Ekran Resmi 2023-03-01 23 44 12" src="https://user-images.githubusercontent.com/116847744/222260778-b596d3f8-1f39-4d9a-a15d-6c73ee2e9a2f.png">

Sorgu 3- film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
Çözüm 3-SELECT COUNT(title) FROM film
WHERE  title ~~ 'T%' AND rating = 'G';
<img width="492" alt="Ekran Resmi 2023-03-01 23 51 25" src="https://user-images.githubusercontent.com/116847744/222262209-a4f9b1e4-b7bb-4719-b398-165353a54282.png">

Sorgu 4- country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
Çözüm 4-SELECT COUNT(country) FROM country
WHERE country ~~ '_____';
<img width="509" alt="Ekran Resmi 2023-03-01 23 54 36" src="https://user-images.githubusercontent.com/116847744/222262799-d61d43e2-4d2c-4238-8d7f-e6bbc8d2a5a8.png">

Sorgu 5- city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
Çözüm 5-SELECT COUNT(city) FROM city
WHERE city ~~* '%r';<img width="519" alt="Ekran Resmi 2023-03-01 23 56 45" src="https://user-images.githubusercontent.com/116847744/222263215-682ccb52-aed0-488b-9ddb-0c4ad2a16b86.png">
