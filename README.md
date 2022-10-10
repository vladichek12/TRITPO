# Требования к проекту
---

# Содержание
1 [Введение](#intro)  
1.1 [Назначение](#appointment)  
1.2 [Бизнес-требования](#business_requirements)  
1.2.1 [Исходные данные](#initial_data)  
1.2.2 [Возможности бизнеса](#business_opportunities)  
1.2.3 [Границы проекта](#project_boundary)  
1.3 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)  
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.1 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Загрузка информации о книгах](#books_downloading)  
3.1.1.2 [Добавление новых книг](#add_book)  
3.1.1.3 [Добавление новых пользователей](#add_user)  
3.1.1.4 [Составление актов выдачи и приема книг](#book_lending&acceptance)  
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)  
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  

<a name="intro"/>

# 1 Введение

<a name="appointment"/>

## 1.1 Назначение
Документ разработан для однозначной трактовки требований между разработчиком и заказчиком. Необходимо разработать web приложение для автоматизации работы библиотекаря. Необходимо, чтобы приложение имело главную страницу со списком всех книг, что есть в библиотеке Вторая страница - форма регистрации нового читателя. Третья - форма регистрации нововй книги. Четвертая - форма для акта выдачи книги. Пятая - форма для акта приема книги.
В этом документе описаны функциональные и нефункциональные требования к кроссплатформенному web приложению «Library». 
Этот документ предназначен для команды, которая будет реализовывать и проверять корректность работы приложения. 

<a name="business_requirements"/>

## 1.2 Бизнес-требования

<a name="initial_data"/>

### 1.2.1 Исходные данные
В настоящее время происходит масштабная автоматизация бизнес-процессов на многих предприятиях. Ручное заполнение документации библиотекарем(регистрация книг и читателей, составление актов выдачи и приема книг) занимает много времени. Следовательно, эти процессы можно автоматизировать.

<a name="business_opportunities"/>

### 1.2.2 Возможности бизнеса
На данный момент на многих предприятиях происходит автоматизация всех рабочих процессов. Для удобства работников и повышения производительности многие процессы переводятся с ручного труда на компьютерную обработку. Таким образом, данное программное обеспечение создается для автоматизации труда библиотекарей.

<a name="project_boundary"/>

### 1.2.3 Границы проекта
Приложение не требует регистрации.
Приложение «Library» позволит пользователям просматривать в режиме реального времени информацию о книгах, что есть в наличии, регистрировать новые книги и читателей, а так же составлять акты выдачи и приема книг. 

<a name="analogues"/>

## 1.3 Аналоги
Аналогом для данного приложения может выступать любое корпоративное CRUD-приложение, призванное автоматизировать труд работников предприятий, не только библиотекарей. В открытом доступе примеров таких приложений нет, так как они предназначены не для общего пользования, а для корпоративного.

<a name="user_requirements"/>

# 2 Требования пользователя

<a name="software_interfaces"/>

## 2.1 Программные интерфейсы
Продукт должен являться web-приложением и иметь удобное  оформление. Front-end часть должна быть создана средствами HTML/CSS. Серверная часть должна быть написана на Java Servlets API.

<a name="user_interface"/>

## 2.2 Интерфейс пользователя
Стартовое окно приложения.

![Главное окно приложения](https://github.com/vladichek12/TRITPO/blob/main/sapmples/main.jpg)  
Главное окно приложения.   
![Форма регистрации книг](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_registration.jpg)  
Окно для регистрации книг потсупивших в библиотеку 
![Форма регистрации книг](https://github.com/vladichek12/TRITPO/blob/main/sapmples/reader_registration.jpg)  
Окно для регистрации новых читателей
![Форма регистрации книг](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_lending.jpg)  
Окно для составления акта выдачи книги 
![Форма регистрации книг](https://github.com/vladichek12/TRITPO/blob/main/sapmples/book_acceptance.jpg)  
Окно для составления акта приема книги


## 2.3 Характеристики пользователей

<a name="user_classes"/>

### 2.3.1 Классы пользователей

Приложение является корпоративным, его пользователем может стать только библиотекарь

<a name="application_audience"/>

### 2.3.2 Аудитория приложения

<a name="target_audience"/>

#### 2.3.2.1 Целевая аудитория
Библиотекари

<a name="collateral_audience"/>

#### 2.3.2.2 Побочная аудитория
Из-за того, что приложение корпоративное, побочная аудитория отсутствует

<a name="assumptions_and_dependencies"/>

## 2.4 Предположения и зависимости
1. Приложение не работает при отсутствии подключения к Интернету;
2. Приложение не работает без предустановленных JRE14 и PgAdmin4.

<a name="system_requirements"/>

# 3 Системные требования

<a name="functional_requirements"/>

## 3.1 Функциональные требования

<a name="main_functions"/>

### 3.1.1 Основные функции

<a name="books_downloading"/>
#### 3.1.1.1 Загрузка информации о книгах
**Описание.** После запуска приложения на экране

| Функция | Требования | 
|:---|:---|
| Загрузка информации о книгах, на данных момент находящихся в наличии | Приложение должно загрузить список книг из базы данных, после запуска приложения пользователем |

<a name="add_book"/>
#### 3.1.1.2 Добавление новых книг
**Описание.** После перехода на соответствующую вкладку

| Функция | Требования | 
|:---|:---|
| Добавление новой книги в базу данных библиотеки | Приложение должно правильно сохранить зарегистрированную книгу в базе данных |

<a name="add_user"/>
#### 3.1.1.3 Добавление новых пользователей
**Описание.** После перехода на соответствующую вкладку

| Функция | Требования | 
|:---|:---|
| Добавление нового пользователя в базу данных библиотеки | Приложение должно правильно сохранить зарегистрированного пользователя в базе данных |

<a name="book_lending&acceptance"/>
#### 3.1.1.4 Составление актов выдачи и приема книг
**Описание.** После перехода на соответствующую вкладку

| Функция | Требования | 
|:---|:---|
| Составление актов выдачи и приема книг | Приложение должно отобразить акт выдачи/приема книги как на экране пользователя, так и в базе данных библиотеки  |

<a name="restrictions_and_exclusions"/>

### 3.1.2 Ограничения и исключения
1. Приложение работает только при наличии подключения к Интернету;
2. Приложение работает только с СУБД postgreSQL.

<a name="non-functional_requirements"/>

## 3.2 Нефункциональные требования

<a name="quality_attributes"/>

### 3.2.1 Атрибуты качества

<a name="requirements_for_ease_of_use"/>

#### 3.2.1.1 Требования к удобству использования
1. Доступ к основным функциям приложения не более чем за две операции;
2. Все функциональные элементы пользовательского интерфейса имеют названия, описывающие действие, которое произойдет при выборе элемента;
3. Обновление информации о книгах в наличии сразу после их регистрации.
4. Обновление информации о количестве экземпляров книг сразу после составления акта приема.

<a name="security_requirements"/>

#### 3.2.1.2 Требования к безопасности
Приложение должно шифровать личные данные пользователей перед записью в базу данных.

<a name="external_interfaces"/>

### 3.2.2 Внешние интерфейсы
  * размер шрифта не менее 12пт;
  * сочетание цветов интерфейса.
  * удобное расположение кнопок.

<a name="restrictions"/>

### 3.2.3 Ограничения
1. Дизайн должен соответствовать пункту интерфейс пользователя.
2. Приложение должно быть написано на Java 8(JDBC и ServletsApi)
3. В качечтве СУБД необходимо использовать PostgreSQL.
