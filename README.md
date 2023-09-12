# LIBRARY
SQL

Идея проекта
Библиотечная система управления - это проект, направленный на создание эффективной системы управления деятельностью библиотеки. Эта система позволяет пользователям выпускать книги, искать различные книги и их названия, предоставляет подробную информацию о книгах,их рейтингах и о количестве скачиваний, доступных в библиотеке, а также о работниках,каждый из которых несет единоличную отвественность за конкретную категорию книг. Автоматизируя эти процессы, он устраняет необходимость ручного ведения учета и предлагает удобный интерфейс.

Таблица: книги

Столбцы:
идентификатор	-	Уникальный идентификатор книги,
титул		   -     Название книги,
автор		 -       Автор книги,
категория	-	    Категория книги,
цена     -  	    Цена книги,
статус	 -     	Статус книги (например, доступна, продана),
всего_копий 	-	Общее количество доступных копий;

Таблица: клиенты
(В таблице хранится информация о клиентах библиотеки)


Столбцы:

идентификатор	      -            	Уникальный идентификатор клиента,
first_name		     -               Имя заказчика,
last_name	        -                Фамилия заказчика,
Отправить по электронной почте	-  Адрес электронной почты клиента,
Номер телефона    -              	Номер телефона заказчика;


Таблица: issued_books
(В таблице хранится информация о книгах, выданных покупателями)

Столбцы;

идентификатор		-  Уникальный идентификатор выданной книги,
book_id		    -    Книги со ссылками на внешние ключи (id),
customer_id  -   	Внешние ключи со ссылкой на клиентов (id),
issue_date	  -  	Дата выхода книги,
due_date	  -      Срок возврата книги,
return_date		-    Дата возврата книги (необязательно);


Таблица:staff
(В таблице хранится информация о персонале)

Столбцы:

id    -  Уникальный идентификатор работника,
name   - ФИО работника,
c      - Категория книг за которую отвечает конкретный работник(1 категории соответствует 1 работник);

Таблица:rating
(В таблице хранится информация о рейтинге книг)

Столбцы:

book_id   -Уникальный идентификатор книги,
rating   - Рейтинг книги,
count     -Количество скачиваний;


Заключение
Библиотечная система управления — это автоматизированное решение, упрощающее управление книгами в библиотеке. Он предлагает удобный интерфейс, обширные сведения о книгах и эффективные функции поиска. Используя SQL-запросы, он взаимодействует с базой данных для эффективного хранения и извлечения информации. Благодаря этой системе процесс управления книгами становится более упорядоченным и удобным как для сотрудников библиотеки, так и для пользователей. 
