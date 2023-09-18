# Fruit bazar
1. Склонировать репозиторий
```
git clone git@github.com:AnastasiyaGapochkina01/fruit_bazar.git ecommerce
```
2. Создать базу данных, настроить пользователя с правами, залить дамп

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
3. Настроить nginx
```
$ sudo cp ecommerce /etc/nginx/sites-enabled/ecommerce
$ sudo ln -s /etc/nginx/sites-available/ecommerce /etc/nginx/sites-enabled
$ nginx -t
$ nginx -s reload
```
4. Преднастроенные (дефолтные) учетные записи
```
admin access:
saifulislamsapon@gmail.com
pass:1234

user access:
saifulislamsapon@gmail.com
123
```
