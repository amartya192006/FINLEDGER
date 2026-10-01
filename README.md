# FINLEDGER
# Finledger is a payment app.

# WORKFLOW
DATABASE MYSQL USED 
TABLE 1 (USERS)
mysql> describe users;
+---------------+--------------+------+-----+-------------------+-----------------------------------------------+
| Field         | Type         | Null | Key | Default           | Extra                                         |
+---------------+--------------+------+-----+-------------------+-----------------------------------------------+
| user_id       | bigint       | NO   | PRI | NULL              | auto_increment                                |
| full_name     | varchar(100) | NO   |     | NULL              |                                               |
| email         | varchar(255) | NO   | UNI | NULL              |                                               |
| phone         | varchar(15)  | NO   | UNI | NULL              |                                               |
| password_hash | text         | NO   |     | NULL              |                                               |
| is_active     | tinyint(1)   | NO   |     | 1                 |                                               |
| created_at    | timestamp    | NO   |     | CURRENT_TIMESTAMP | DEFAULT_GENERATED                             |
| updated_at    | timestamp    | NO   |     | CURRENT_TIMESTAMP | DEFAULT_GENERATED on update CURRENT_TIMESTAMP |
+---------------+--------------+------+-----+-------------------+-----------------------------------------------+
8 rows in set (0.008 sec)
