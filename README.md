# Урок 7: API (Google Sheets, Яндекс.Метрика)

## Описание урока

В этом уроке изучаются практические навыки работы с API, а также дополнительные функции и методы для обработки данных, с которыми мы познакомились в лекциях. В уроке задействованы данные из Google Sheets, Яндекс.Метрики, а также тестовые данные для отработки типичных задач на работу с API.

## Задачи

1. **Чтение данных из Google Sheets и анализ данных посетителей**
   - Получите данные из Google Sheets с помощью библиотеки `requests`.
   - Подсчитайте процент мужчин среди всех посетителей сайта и округлите результат до целых.

2. **Работа с данными посещаемости из Яндекс.Метрики**
   - Скачайте файл с данными посещаемости сайта из Яндекс.Метрики и загрузите его в DataFrame (`df`).
   - Используя функцию `np.where`, создайте серию `chrome_robots`, в которую будет записываться 1, если посещение сайта было сделано роботом с браузера, содержащего 'Chrome' в названии, и 0 в других случаях.

3. **Работа с датасетом кликов и показов по объявлениям**
   - Используйте датасет с данными о кликах и показах, в котором возможны пропуски значений.
   - Подсчитайте количество строк без пропусков в колонке `click_type` и сохраните результат в переменную `not_nan_count`.

4. **Работа со списками и обработка исключений**
   - Дан список `lst` с разными элементами.
   - Используя `try-except` в цикле, попытайтесь преобразовать каждое значение в списке в `int`. Если преобразование удалось, добавьте значение в новый список `new_list`.

5. **Отправка сообщения с помощью Telegram API**
   - Используя Telegram API, отправьте сообщение себе в личный чат.
   - В ответ на выполнение задачи укажите ник бота, который будет отправлять сообщение.

## Данные

### Датасеты, используемые в задачах:
- **Google Sheets** — данные из Google Sheets, содержащие информацию о посетителях сайта.
- **Яндекс.Метрика** — данные посещаемости сайта из Яндекс.Метрики, сохраненные в переменной `df`.
- **Датасет кликов и показов** — содержит данные о взаимодействии пользователей с рекламными объявлениями.

#### Структура датасета кликов и показов:
- **ad_id**: ID объявления
- **user_id**: ID пользователя
- **click_type**: Тип клика (например, клик по заголовку объявления, клик по центру)

## Выводы

Задачи урока охватывают базовые операции для работы с API и показывают, как использовать запросы к сервисам, обрабатывать данные и внедрять исключения в коде. Полученные навыки пригодятся для работы с внешними API и обработки данных в реальных проектах.


# Lesson 7: API (Google Sheets, Yandex.Metrica)

## Lesson Description

In this lesson, we will study practical skills for working with APIs, as well as additional functions and methods for processing data that we have learned in previous lectures. The lesson involves data from Google Sheets, Yandex.Metrica, and also test data for practicing typical API-related tasks.

## Tasks

1. **Reading Data from Google Sheets and Visitor Data Analysis**
   - Retrieve data from Google Sheets using the `requests` library.
   - Calculate the percentage of male visitors among all website visitors and round the result to the nearest whole number.

2. **Working with Yandex.Metrica Traffic Data**
   - Download the website traffic data file from Yandex.Metrica and load it into a DataFrame (`df`).
   - Using the `np.where` function, create a series called `chrome_robots`, where 1 is recorded if a site visit was made by a bot using a browser with 'Chrome' in the name, and 0 in other cases.

3. **Working with Click and Impression Dataset**
   - Use the dataset with click and impression data, which may contain missing values.
   - Count the number of rows without missing values in the `click_type` column and save the result in the variable `not_nan_count`.

4. **Working with Lists and Exception Handling**
   - Given a list `lst` with various elements.
   - Using `try-except` in a loop, attempt to convert each value in the list to `int`. If the conversion is successful, add the value to a new list `new_list`.

5. **Sending a Message Using Telegram API**
   - Using the Telegram API, send a message to yourself in a personal chat.
   - In response to completing the task, provide the bot username that will send the message.

## Data

### Datasets Used in the Tasks:
- **Google Sheets** — data from Google Sheets containing information about website visitors.
- **Yandex.Metrica** — website traffic data from Yandex.Metrica, stored in the variable `df`.
- **Click and Impression Dataset** — contains data on user interactions with advertising banners.

#### Structure of the Click and Impression Dataset:
- **ad_id**: Ad ID
- **user_id**: User ID
- **click_type**: Type of click (e.g., click on the ad title, click on the ad center)

## Conclusions

The tasks of this lesson cover basic operations for working with APIs and demonstrate how to make requests to services, process data, and implement exceptions in the code. The skills gained will be useful for working with external APIs and processing data in real-world projects.

