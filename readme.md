
mysql> create database hotel;
Query OK, 1 row affected (0.156 sec)

mysql> use hotel;
Database changed
mysql> CREATE TABLE reservations (
    ->     reservation_id INT PRIMARY KEY AUTO_INCREMENT,
    ->     guest_name VARCHAR(100),
    ->     contact_no VARCHAR(15),
    ->     room_no INT,
    ->     check_in_time TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    ->     check_out_time TIMESTAMP
    -> );
Query OK, 0 rows affected (0.450 sec)

mysql> select*from reservations;
Empty set (0.366 sec)

mysql> select*from reservations;
+----------------+------------+------------+---------+---------------------+----------------+
| reservation_id | guest_name | contact_no | room_no | check_in_time       | check_out_time |
+----------------+------------+------------+---------+---------------------+----------------+
|              1 | anurag     | 7894409727 |      69 | 2026-01-31 16:07:04 | NULL           |
+----------------+------------+------------+---------+---------------------+----------------+
1 row in set (0.308 sec)
