# Fruit bazar
First create a database name ecommerce in your database. Than import ecommerce.sql file in your ecommerce database.

```
$ sudo mysql
> create database ecommerce;
> create user 'ecom'@'%' identified by 'ecompasswd';
> grant usage on *.* to 'ecom'@'%';
> grant all privileges on ecommerce.* to 'ecom'@'%';
> flush privileges;
> exit
$ sudo mysql ecommerce < ecommerce.sql
```
2
admin access:
saifulislamsapon@gmail.com
pass:1234


user access:
saifulislamsapon@gmail.com
123
