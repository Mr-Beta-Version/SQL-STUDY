# SQL-STUDY

```
UNION
```
UNION MARGE 2 data together.
Example:

```
SELECT username FROM users
UNINO
SELECT username FROM admins;
```
It will show table1 and table2 data on page

visual of table
```
Table: users              Table: admins
+---------+               +---------+
| username|               | username|
+---------+               +---------+
| alice   |               | root    |
| bob     |               | walid   |
| charlie |
+---------+               +---------+

        UNION SELECT

             ↓

Combined Result
+---------+
| username|
+---------+
| alice   |
| bob     |
| charlie |
| root    |
| walid   |
+---------+

```




