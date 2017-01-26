
### Types:
* Integer
* Text
* Date
* Real

```NULL``` - is a specific value in SQL that represents missing or unknown data.

**create table:**
```sql
CREATE TABLE celebs (id INTEGER, name TEXT, age INTEGER);
```
**select data:**
```sql
SELECT * FROM celebs

SELECT name, imdb_rating FROM movies;

SELECT * FROM movies WHERE imdb_rating > 8;

SELECT * FROM movies WHERE year BETWEEN 1990 AND 2000;

SELECT * FROM movies
WHERE year BETWEEN 1990 AND 2000
AND genre = 'comedy';

SELECT * FROM movies
WHERE genre = 'comedy'
OR year < 1980;

SELECT * FROM movies
ORDER BY imdb_rating DESC;

SELECT * FROM movies
ORDER BY imdb_rating ASC
LIMIT 3;
```

**get unique values:**
```sql
SELECT DISTINCT genre FROM moves;

```
**regex:**
```sql
SELECT * FROM movies
WHERE name LIKE 'Se_en';
```

**add a row:**
```sql
INSERT INTO celebs (id, name, age) VALUES (1, 'Justin Bieber', 21);
```
**edits a row:**
```sql
UPDATE celebs
SET age = 22
WHERE id = 1;
```
**add a new column:**
```sql
ALTER TABLE celebs ADD COLUMN twitter_handle TEXT;
```

**delete a row:**
```sql
DELETE FROM celebs WHERE twitter_handle IS NULL;

```
