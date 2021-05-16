mysql 계정(account) 만들기 
계정(account)
id : ace
pw : 1234
사용DB : acedb

*******************************************

mysql> use mysql
mysql> show  tables;
mysql> create  database acedb;
mysql> show  databases;

mysql> create  user ace@'%' identified by '1234';
mysql> grant all privileges on acedb.*  to  ace@'%' with grant option;
mysql> flush  privileges;


 
ace 계정으로 접속하기
환경변수에 등록하기 
시스템 path에 C:\Program Files\MySQL\MySQL Server 8.0\bin  등록 

명령프롬프트에서 접속

>mysql  -u  ace  -p1234

DDL(Data Definition Language)
 create 
 alter
 drop 

DML(Data Manipulation Language)
 insert
 delete
 update
 select 

DCL(Data Control Language)
 grant
 revoke 
 commit
 rollback 
