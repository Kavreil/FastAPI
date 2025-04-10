## Описание проекта

Проект представляет собой RESTful API, разработанный с использованием фреймворка FastAPI , для управления базой данных компьютерных комплектующих. API предоставляет возможности для получения списка комплектующих, добавления новых элементов, поиска по идентификатору и расчета стоимости элементов в базе данных.
* * *
Создание БД:
Формируется БД с различными комплектующими для ПК со своими уникальными характеристиками.
* * *
Получение списка комплектующих :
Маршрут /api/pc возвращает список всех комплектующих, хранящихся в базе данных.
Каждый элемент содержит информацию о типе, производителе, модели, стоимости, описании и уникальном идентификаторе.
* * *
Расчет общей стоимости :
Маршрут /api/pc/total вычисляет и возвращает общую стоимость всех комплектующих в базе данных.
* * *
Поиск комплектующих по ID :
Маршрут /api/pc/{id} позволяет получить информацию о конкретном комплектующем по его уникальному идентификатору.
Если комплектующее не найдено, возвращается статусный код 404 с сообщением об ошибке.
* * *
Добавление новых комплектующих :
Маршрут /api/pc (POST-запрос) позволяет добавлять новые комплектующие в базу данных. Для этого необходимо передать JSON-объект с полями: typePC, vendor, model, cost, description.
* * *
Тестирование API :
Реализованы примеры запросов для тестирования API с использованием библиотеки requests.
Добавлено взаимодействие с пользователем через консоль для ввода данных нового комплектующего.
