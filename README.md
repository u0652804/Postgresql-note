# Postgresql-note

### 1. download(Windows) :
 - pgAdmin(base on GUI to control postgreSql) : https://www.postgresql.org/ftp/pgadmin/pgadmin4/v4.24/windows/
 - postgresql : https://www.enterprisedb.com/downloads/postgres-postgresql-downloads
 
ps : pgAdmin 可以在安裝postgresql時選擇是否安裝,不用先單獨下載 

### 2. install 

install step1 : 
 - checked four items to install
 - edit user and password and record them to a note file such as .txt file
 
install step2 : un checked the item "Stack Builder ..." -> finish

reference : https://www.runoob.com/postgresql/windows-install-postgresql.html

### 3. start psql 

reference : https://www.youtube.com/watch?v=qw--VYLpxG4

execute SQL shell

- enter until password item : key in recorded password 

- when show postgres=#, you can start to use psql cmd

### 4. psql cmds :

ps : Don't delete two default database named template0 and template1

    psql --help : show cmd list

    \l : show all databases

    create databhase $dbName; (e.g. testdb1)(ps : this new database created by copy default db named template1)

    \c $dbName; : connect to the pointed db

    drop database $dbName; : delete db

### 5. start sql cmds :

desc : after \c to connected to a db, can use sql code language to control this db

ex : create a new table and it's cols

    testdb1=# create table test1(
    testdb1(# id int,
    testdb1(# fname varchar(50),
    testdb1(# lname varchar(50),
    testdb1(# sex varchar(5),
    testdb1(# birth date);//xx

    \d : list tables in this db

    \d $tableName : list detail about pointed table

