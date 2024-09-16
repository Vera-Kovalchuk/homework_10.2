 Структура проекта
Структура содержит пакеты 
src
 и 
tests
, файл 
main.py
, артефакты Poetry (файлы 
pyproject.toml
 и 
poetry.lock
).
Создан модуль 
masks
 в пакете 
src
.
 Реализация функций
Функция 
get_mask_card_number
 принимает на вход номер карты в виде числа и возвращает маску номера по правилу 
XXXX XX** **** XXXX
.
Функция 
get_mask_account
 принимает на вход номер счета в виде числа и возвращает маску номера по правилу 
**XXXX
.
 Работа с линтерами и форматерами
Все библиотеки установлены в группу зависимостей 
lint
.
В репозитории есть файл 
.flake8
 с конфигурацией, параметр 
max-line-length
 равен 119 символам, в параметре 
exclude
 учтены папки 
.git
, 
__pycache__
.
В файле 
pyproject.toml
 прописана конфигурация 
black
, параметр 
line-length
 равен 119 символам, в параметре 
exclude
 учтена папка 
.git
.
В файле 
pyproject.toml
 прописана конфигурация 
isort
, параметр 
line_length
 равен 119 символам.
При вызове 
isort
 форматируется не более 1 импорта.
В файле 
pyproject.toml
 прописана конфигурация 
mypy
, параметр 
disallow_untyped_defs
 равен 
true
, параметр 
warn_return_any
 равен 
true
, в параметре 
exclude
 учтена папка 
venv
.
 Оформление кода
При запуске линтеров Flake8 и 
mypy
 выдается не более 2 ошибок.
Для всех реализованных функций написаны docstring.
Для параметров и возвращаемых значений функции описаны корректные аннотации типов.
Нейминг функций отвечает правилам оформления кода PEP 8.
Все функции названы в соответствии с условиями задания.