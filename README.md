# tmdb_api. Упражнение на чтение кода. Фильмы с TMDB

## Какой фильм посмотреть? `find_similar.py`

Скрипт запрашивает от пользователя:
- `path` - путь до базы данных;
- `keyword` - название искомого фильма

Результатом программы является вывод рекомендуемых фильмов

## Вывод запроса на TMBD (тестовый) `hello_api_TMDB.py`

Получает API-ключ `user_api_key` от пользователя и возвращает десеариализированный словарь результата запроса на TMDB

## Создание базы данных фильмов `make_own_db.py`

Создает базу данных на основании запроса на TMDB, который возвращает определенное количество фильмов 'films_amount' (по умолчанию 1000). Полученные данные записываются в базу данных `MyFilmDB.json`

## Получение существующей базы данных фильмов `own_db_helpers.py`

Содержит в себе функцию `load_data`, принимающая путь `path`.
Функция возвращает `None`, если пути не существует или возвращает базу данных

## Поиск фильма в базе данных `search_in_db.py`

Скрипт запрашивает от пользователя:
- `path` - путь до базы данных;
- `keyword` - название искомого фильма

Возвращает кортеж фильмов с названием указанным в `keyword`

## `tmdb_helpers.py`

Модуль содержит в себе вспомогательные методы для работы с запросами к TMDB.

1. `make_tmdb_api_request`
Отправляет запрос на TMDB API, возвращает десеариализированный словарь запроса

2. `load_json_data_from_url` 
Возвращает десеариализированный словарь запроса

3. `get_user_api`
Получает от пользователя API-ключ от TMDB


