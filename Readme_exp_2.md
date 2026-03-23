---> Exercise 2: Filtering queries

Question:1 Find the movie with a row id of 6

```sql 
SELECT * FROM movies
WHERE id = 6;
```

| ID | Title           | Director  | Year | Length (Minutes) |
| -- | --------------- | --------- | ---- | ---------------- |
| 6  | The Incredibles | Brad Bird | 2004 | 116              |

Question:2 Find the movies released in the years between 2000 and 2010

```sql
SELECT title, year FROM movies
WHERE year BETWEEN 2000 AND 2010;
```
| Title           | Year |
| --------------- | ---- |
| Monsters, Inc.  | 2001 |
| Finding Nemo    | 2003 |
| The Incredibles | 2004 |
| Cars            | 2006 |
| Ratatouille     | 2007 |
| WALL-E          | 2008 |
| Up              | 2009 |
| Toy Story 3     | 2010 |

Question:3 Find the movies not released in the years between 2000 and 2010

```sql
SELECT title, year FROM movies WHERE year NOT BETWEEN 2000 AND 2010;
```
| Title               | Year |
| ------------------- | ---- |
| Toy Story           | 1995 |
| A Bug's Life        | 1998 |
| Toy Story 2         | 1999 |
| Cars 2              | 2011 |
| Brave               | 2012 |
| Monsters University | 2013 |


Question:4 Find the first 5 Pixar movies and their release year

```sql
SELECT title, year FROM movies
ORDER BY year ASC
LIMIT 5;
```

| Title          | Year |
| -------------- | ---- |
| Toy Story      | 1995 |
| A Bug's Life   | 1998 |
| Toy Story 2    | 1999 |
| Monsters, Inc. | 2001 |
| Finding Nemo   | 2003 |





