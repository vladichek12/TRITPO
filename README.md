# Требования к проекту 
# Содержание 
[1 Введение](https://github.com/vladichek12/TRITPO/blob/main/README.md#1-введение)  
[2 Требования пользователя](https://github.com/vladichek12/TRITPO/blob/main/README.md#2-требования-пользователя)  
[2.1 Программные интерфейсы](https://github.com/vladichek12/TRITPO/blob/main/README.md#21-программные-интерфейсы)  
[2.2 Интерфейс пользователя](https://github.com/vladichek12/TRITPO/blob/main/README.md#22-интерфейс-пользователя)  
[2.3 Характеристики пользователя](https://github.com/vladichek12/TRITPO/blob/main/README.md#23-характеристики-пользователей)  
[2.4 Предположения и зависимости](https://github.com/vladichek12/TRITPO/blob/main/README.md#24-предположения-и-зависимости)  
[3 Системные требования](https://github.com/vladichek12/TRITPO/blob/main/README.md#3-системные-требования)  
[3.1 Функциональные требования](https://github.com/vladichek12/TRITPO/blob/main/README.md#31-функциональные-требования)  
[3.2 Нефункциональные требования](https://github.com/vladichek12/TRITPO/blob/main/README.md#32-нефункциональные-требования)  
[3.2.1 Атрибуты качества](https://github.com/vladichek12/TRITPO/blob/main/README.md#321-атрибуты-качества)  
[3.2.2 Требования к безопасности](https://github.com/vladichek12/TRITPO/blob/main/README.md#322-требования-к-безопасности)  
[3.2.3 Ограничения](https://github.com/vladichek12/TRITPO/blob/main/README.md#323-ограничения)
## 1 Введение  
Задумкой проекта является создание web-сервиса "Библиотека". Библиотекарь является пользователем приложения. Он может просматривать список книг, регистрировать новые книги и новых читателей, а так же оформлять акты выдачи и приема книг. 
## 2 Требования пользователя  
## 2.1 Программные интерфейсы 
Продукт должен иметь web-интерфейс. Для этого будут использован Java Servlet API. Все данные  (списки читателей, книг, жанров книг) будут храниться в базе данных postgre sql. Приложение должно быть написано на языке программирования Java.  
## 2.2 Интерфейс пользователя  
## Окно пользователя  
Главная вкладка "Книги"  
![](https://github.com/vladichek12/TRITPO/blob/main/sapmples/main.jpg)  
Вкладка "Регистрация книг" в которой происходит регистрация книг  
![](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_registration.jpg) 
Вкладка "Регистрация читателей" в которой происходит регистрация читателей  
![](https://github.com/vladichek12/TRITPO/blob/main/sapmples/reader_registration.jpg) 
Вкладка "Выдача книг" в которой происходит регистрация акта выдачи книг  
![](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_lending.jpg) 
Вкладка "Прием книг" в которой происходит регистрация акта приема книг  
![](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_acceptance.jpg) 
## 2.3 Характеристики пользователей  
Пользователь приложения - библиотекарь. Это человек, занимающийся регистрацией книг и читалей, составлением актов выдачи и приема книг.
## 2.4 Предположения и зависимости 
Для приложения требуется компьютер, сеть интернет, 4мБ памяти.
## 3 Системные требования  
Приложение требует установленного сервиcа для работы с базой данных postgreSQL PgAdmin 4, JRE 14(Java Runtime Environment), 4мБ памяти.
## 3.1 Функциональные требования 
1.Просмотр списка книг  
2.Добавление новых книг
3.Добавление новых читателей  
4.Выдача книг  
5.Прием книг  
## 3.2 Нефункциональные требования  
## 3.2.1 Атрибуты качества
Атрибуты важные для пользователя:  
1.Удобство в использовании  
2.Понятный и приятный интерфейс   
3.Легкость редактирования ошибок
4.Удобвство в расширении проекта
## 3.2.2 Требования к безопасности  
Личные данные покупателя при сохранении в базу данных должны кодироваться. 
## 3.2.3 Ограничения    
Язык программирования Java,РСУБД postgreSQL, дизайн должен соответствовать пункту интерфейс пользователя.
