Дипломный проект: реальный кейс компании «Ростелеком Информационные Технологии»
Обьекты тестирования: форма авторизации сайта "Ростелеком" (https://b2c.passport.rt.ru)
Техники тестирования, которые использовались:
при создании тестовых данных для полей использовалась техника разбиения на классы эквивалентности и граничные значения. Также использовалась техника предугадывания ошибок.
Структура проекта:
- папка data_for_negative_test с файлом data_for_test.py -  данные для ввода: почта, пароль, имя, фамилия, а также символы, 255 символов и тд.
- папка locators с файлом page_locators.py - наиболее часто используемые локаторы
- папка pages с файлами: base_page.py - основные функции, используемые в каждом тесте: открыть главную страницу сайта и функция ожидания видимости элемента; page.py - функции заполнения полей и функции открытия некоторых ссылок
- папка tests с файлами: conftest.py - содержит фикстуру, в файле использовалась библиотека webdriver-manager для автоматического поиска или скачивания драйвера; test_authorization_negative - негативные тесты формы авторизации; test_positive - позитивные тесты на форму авторизации и регистрации, так же на ссылки, чек бокс и тд; tests_registration_negative - негативные тесты формы регистрации.
