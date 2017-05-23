codeanywhere資料庫使用

![img](img/01.png)
滑鼠對建立好的連線點擊右建，選擇SSH Terminal
***
![img](img/02.png)
在文字框內輸入

`mysql -u root -p`

登入
***
![img](img/03.png)
詢問密碼，預設為空直接Enter
***
![img](img/04.png)
更改密碼

`SET PASSWORD FOR 'root'@'localhost' = PASSWORD('password');`

***
![img](img/05.png)
查詢成功
***
![img](img/06.png)
更新相關權限

`flush privileges;`

***
![img](img/07.png)
查詢成功
***
![img](img/08.png)
顯示現有資料庫

`show databases;`

***
![img](img/09.png)
查詢成功畫面
***
![img](img/10.png)
建立新資料庫

`create database test_db;`

***
![img](img/11.png)
選擇資料庫

``use `test_db`;``

***
![img](img/12.png)
建立資料表

`CREATE TABLE test_tbl(`

`id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,`

`usr_name VARCHAR(30) NOT NULL,`

`email VARCHAR(50)`

`);`

***
![img](img/13.png)
查詢資料表

``select * from `test_tbl`;``

***
![img](img/14.png)
查詢成功
***
![img](img/15.png)
輸入資料內容

`INSERT INTO test_tbl (usr_name,email)`

`VALUES ('name_01','name_01@email');`

***
![img](img/16.png)
查詢資料表

``select * from `test_tbl`;``

***
![img](img/17.png)
查詢成功之畫面
***
