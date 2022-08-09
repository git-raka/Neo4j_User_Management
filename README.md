# Neo4j_User_Management

## PREPARATION
CREATE DATABASE <database-name>

*CREATE USER <user-name>


SET PASSWORD "<password>"

SET PASSWORD CHANGE NOT REQUIRED

SET STATUS ACTIVE

SET HOME DATABASE <database-name>;*

GRANT ROLE architect TO <username>;

## USER MANAGEMENT
SHOW USERS

SHOW CURRENT USER;

SHOW USERS;

![image](https://user-images.githubusercontent.com/77326619/183657037-89869f92-dc94-4d6f-bec2-41917de5dacf.png)

![image](https://user-images.githubusercontent.com/77326619/183657045-413f6d12-6769-49c9-aaa4-8e1cd9add210.png)

SHOW USERS YIELD user, suspended, passwordChangeRequired, roles, home
WHERE user = 'auth1a'

![image](https://user-images.githubusercontent.com/77326619/183657091-4be7b934-aa0f-4795-b74c-df62fa1bbf1c.png)

## CREATE USER
CREATE OR REPLACE USER auth1a
 
 SET PASSWORD "ifgpoc"
 
 SET PASSWORD CHANGE NOT REQUIRED
 
 SET STATUS ACTIVE
 
 SET HOME DATABASE auth1;

![image](https://user-images.githubusercontent.com/77326619/183657191-3c4e1e12-8f35-4fb5-a3e8-3508241f7441.png)

RENAME USER auth1c TO auth1d;

![image](https://user-images.githubusercontent.com/77326619/183657241-faf66803-381a-4b04-af13-4cbd28c56c70.png)

ALTER USER auth1d SET PASSWORD 'abc123' CHANGE NOT REQUIRED SET STATUS ACTIVE;

![image](https://user-images.githubusercontent.com/77326619/183657262-dc8b7d8b-4e7a-45c9-929f-f977c554c5e1.png)


## DROP USER

DROP USER auth1b;

![image](https://user-images.githubusercontent.com/77326619/183657351-0fe70855-ee9f-4533-84ac-2e28dfe95b33.png)

![image](https://user-images.githubusercontent.com/77326619/183657376-5c107d7b-405e-412e-8995-2138b9ad9dc3.png)


