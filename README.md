### Review 1 

```SQL 
1. SELECT * FROM north_american_cities WHERE Country LIKE "Canada";
2. SELECT * FROM north_american_cities WHERE Country LIKE "United States" ORDER BY Latitude DESC;
3. SELECT * FROM north_american_cities WHERE Longitude < (SELECT Longitude FROM north_american_cities WHERE City = 'Chicago') ORDER BY Longitude;
4. SELECT * FROM north_american_cities WHERE Country = "Mexico" ORDER BY Population DESC LIMIT 2;
5. SELECT * FROM north_american_cities WHERE Country = 'United States' ORDER BY Population DESC LIMIT 2 OFFSET 2;
```


### Review 2

```SQL 
1. SELECT Director, Count(Title) FROM movies GROUP BY DIRECTOR;
2. SELECT Director, SUM(Domestic_sales + International_sales) FROM movies INNER JOIN boxoffice ON movies.id = boxoffice.movie_id GROUP BY DIRECTOR;
```

### Case 1

An illegal site's servers were seized in a recent operation. Please submit all users' details.

```SQL 
SELECT * FROM users;
```


### Case 2

An illegal site's servers were seized in a recent operation. Please submit all users' details.

```SQL 
SELECT * FROM users;
```

### Case 3

White hat hacker has sent SQLPD exposed members' details of a shady site connected to various persons of interest. Please submit all members full names, usernames and addresses' details.

```SQL 
SELECT FullName, Username, Address FROM members;
```

### Case 4

White hat hacker has sent SQLPD exposed members' details of a shady site connected to various persons of interest. Please submit all subscribers hashed passwords, number of purchases  and mailing addresses' details.

```SQL 
SELECT HashedPassword, Purchases, MailingAddress FROM subscribers;
```

### Case 5

An illegal site's servers were seized in a recent operation. Please submit all users emails' details. Please make sure there are no duplicates.

```SQL 
SELECT DISTINCT Email FROM users;
```

### Case 6

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all entries' details sorted by join dates in ascending order.

```SQL 
SELECT * FROM mailing_list ORDER BY Joined ASC;
```

### Case 7

White hat hacker has sent SQLPD exposed members' details of a shady site connected to various persons of interest. Please submit all members' details sorted by joined on dates in descending order.

```SQL 
SELECT * FROM members ORDER BY JoinedOn DESC;
```

### Case 8

An illegal site's servers were seized in a recent operation. Please submit all users access times, surnames and email addresses' details sorted by email addresses in descending order. Please make sure there are no duplicates.

```SQL 
SELECT DISTINCT EmailAddress, AccessTime, Surname FROM users ORDER BY EmailAddress DESC;
```

### Case 9

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit all records join dates and number of children' details sorted by join dates in ascending order and then by number of children in ascending order.

```SQL 
SELECT JoinDate, Children FROM mailing_list ORDER BY JoinDate ASC, Children ASC;
```

### Case 10

An illegal site's servers were seized in a recent operation. Please submit the top 10 users' details when sorted by last access times in descending order and then by first names in descending order.

```SQL 
SELECT * FROM users ORDER BY LastAccess DESC, FirstName DESC LIMIT 10;
```

### Case 11

A mailing list of an illegal online service was sent to the SQLPD hot-line. Please submit the top 20 entries number of password changes, join dates and first names' details when sorted by number of password changes in ascending order and then by first names in ascending order. Please make sure there are no duplicates. 

```SQL 
SELECT DISTINCT FirstName, PassChangeCount, Joined FROM mailing_list ORDER BY PassChangeCount ASC, FirstName ASC LIMIT 20;
```