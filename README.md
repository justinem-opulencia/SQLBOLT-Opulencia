## Review 1 

```SQL 
1. SELECT * FROM north_american_cities WHERE Country LIKE "Canada";
2. SELECT * FROM north_american_cities WHERE Country LIKE "United States" ORDER BY Latitude DESC;
3. SELECT * FROM north_american_cities WHERE Longitude < (SELECT Longitude FROM north_american_cities WHERE City = 'Chicago') ORDER BY Longitude;
4. SELECT * FROM north_american_cities WHERE Country = "Mexico" ORDER BY Population DESC LIMIT 2;
5. SELECT * FROM north_american_cities WHERE Country = 'United States' ORDER BY Population DESC LIMIT 2 OFFSET 2;
```