## План тестирования возможности записи на обучение профессии "Тестировщик ПО".

### Объект тестирования: обучение профессии "Тестировщик ПО" на веб-сайте [Нетология](https://netology.ru/) c формой записи на курс [Тестировщик ПО](https://netology.ru/programs/qa). 

### Цель тестирования: автоматизация тестирования записи на обучение профессии ["Тестировщик ПО"](https://netology.ru/programs/qa) и заполнение формы.

### Перечень автоматизируемых сценариев:

#### Предусловия:

Переход к форме записи на курс "Тестировщик ПО":

- Открыть стартовую страницу сайта Нетология (https://netology.ru/)

- Есть несколько способов перехода к форме записи на курс:

1. В левом верхнем углу нажать на PopUp `"Каталог курсов"`, навести курсор на категорию `"Программирование"`, нажать на категорию `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

2. В левом верхнем углу нажать на PopUp `"Каталог курсов"`, нажать на категорию `"Программирование"`, нажать на профессию `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

3. На главной странице веб-сайта Нетология нажать на категорию `"Программирование"`,нажать на профессию `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

4. На главной странице веб-сайта Нетология нажать на категорию `"Программирование"`, в поле поиска `"Чему вы хотите научиться?"` каталога курсов ввести "Тестировщик ПО", нажать на курс `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

5. В левом верхнем углу нажать на PopUp `"Каталог курсов"`, нажать на кнопку `"Полный каталог"` , нажать на категорию `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

6. В левом верхнем углу нажать на PopUp `"Каталог курсов"`, нажать на кнопку `"Полный каталог"` , в поле поиска `"Чему вы хотите научиться?"` каталога курсов ввести "Тестировщик ПО", нажать на курс `"Тестировщик ПО"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

#### Тестовые сценарии:

##### Позитивные:

1. Заполнить поле формы "Имя" на кириллице (от 2-ух букв), номер телефона с валидными данными, нажать кнопку `"Записаться"`. Отправка формы успешна.
2. Заполнить поле формы "Имя" на кириллице (от 2-ух букв), номер телефона с валидными данными, нажать кнопку `"Получить консультацию"`. Отправка формы успешна.
3. Заполнить поле формы "Имя" на латинице (от 2-ух букв), номер телефона с валидными данными, нажать кнопку `"Записаться"`. Отправка формы успешна.
4. Заполнить поле формы "Имя" на латинице (от 2-ух букв), номер телефона с валидными данными, нажать кнопку `"Получить консультацию"`. Отправка формы успешна.

##### Негативные:

1. Оставить поля формы записи на курс пустыми, нажать на кнопку `"Записаться"`, форма не отправляется, поля подсвечиваются с ошибкой "Обязательное поле".
2. Оставить поля формы записи на курс пустыми, нажать на кнопку `"Получить консультацию"`, форма не отправляется, поля подсвечиваются с ошибкой "Обязательное поле".
3. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с валидными данными, нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
4. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с валидными данными, нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
5. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов". 
6. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов". 
7. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов". 
8. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов". 
9. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (более 15 цифр) `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов" и ошибка "Номер в формате +9 (999) 999-99-99".
10. Заполнить поле формы "Имя" одной буквой на кириллице, номер телефона с невалидными данными (более 15 цифр) `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов" и ошибка "Номер в формате +9 (999) 999-99-99".
11. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с валидными данными, нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
12. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с валидными данными, нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
13. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
14. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
15. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
16. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов".
17. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (более 15 цифр) `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов" и ошибка "Номер в формате +9 (999) 999-99-99".
18. Заполнить поле формы "Имя" одной буквой на латинице, номер телефона с невалидными данными (более 15 цифр) `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно быть не короче 2 симоволов" и ошибка "Номер в формате +9 (999) 999-99-99".
19. Заполнить поле формы "Имя" спецсимволом, номер телефона с валидными данными, нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
20. Заполнить поле формы "Имя" спецсимволом, номер телефона с валидными данными, нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
21. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
22. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
23. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
24. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв".
25. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (более 15 цифр) `"Записаться"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв" и ошибка "Номер в формате +9 (999) 999-99-99".
26. Заполнить поле формы "Имя" спецсимволом, номер телефона с невалидными данными (более 15 цифр) `"Получить консультацию"`, форма не отправляется, поле "Имя" подсвечивается с ошибкой "Должно состоять из букв" и ошибка "Номер в формате +9 (999) 999-99-99".
27. Заполнить поле формы "Имя" двумя и более буквами на кириллице, ввод номера телефона спецсимволами, нажать кнопку `"Записаться"`, форма не отправляется, ошибка "Номер в формате +9 (999) 999-99-99".
28. Заполнить поле формы "Имя" двумя и более буквами на кириллице, ввод номера телефона спецсимволами, нажать кнопку `"Получить консультацию"`, форма не отправляется, ошибка "Номер в формате +9 (999) 999-99-99".
29. Заполнить поле формы "Имя" двумя и более буквами на латинице, ввод номера телефона спецсимволами, нажать кнопку `"Записаться"`, форма не отправляется, ошибка "Номер в формате +9 (999) 999-99-99".
30. Заполнить поле формы "Имя" двумя и более буквами на латинице, ввод номера телефона спецсимволами, нажать кнопку `"Получить консультацию"`, форма не отправляется, ошибка "Номер в формате +9 (999) 999-99-99".
31. Заполнить поле формы "Имя" двумя и более буквами на латинице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется.
32. Заполнить поле формы "Имя" двумя и более буквами на латинице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется.
33. Заполнить поле формы "Имя" двумя и более буквами на латинице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется.
34. Заполнить поле формы "Имя" двумя и более буквами на латинице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется.
35. Заполнить поле формы "Имя" двумя и более буквами на кирилице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется.
36. Заполнить поле формы "Имя" двумя и более буквами на кирилице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Записаться"`, форма не отправляется.
37. Заполнить поле формы "Имя" двумя и более буквами на кирилице, номер телефона с невалидными данными (более 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется.
38. Заполнить поле формы "Имя" двумя и более буквами на кирилице, номер телефона с невалидными данными (менее 11 цифр), нажать кнопку `"Получить консультацию"`, форма не отправляется.

### Перечень используемых инструментов:

1. `IntelliJ IDEA 2021.3.2` - интегрированная среда разработки ПО для многих языков программирования. Удобная среда подготовки авто-тестов.
2. `Java 11` - объектно-ориентированный язык программирования, оптимальный для написания понятных и наглядных автотестов.
3. `JUnit 5` - инструмент тестирования, среда модульного тестирования для языка программирования Java.
4. `Gradle` - мощная и простая система автоматической сборки проектов, которая используется для упрощения работы с JAVA.
5. `Selenide` - это фреймворк для автоматизированного тестирования веб-приложений на основе Selenium WebDriver, дающий следующие преимущества: изящный API, поддержка AJAX для стабильных тестов, мощные селекторы, простая конфигурация.
6. `Faker` - это библиотека, которая позволяет генерировать случайные данные. С ее помощью можно заполнить таблицы в базе данных, построить корректные XML-документы, сформировать JSON-ответы для REST.

### Перечень необходимых разрешений/данных/доступов:

1. Необходимо разрешение на проведение тестирования и автоматизации на веб-сайте [Нетология](https://netology.ru/)
2. Нужен доступ к API и БД (доступ к действующей базе данных несет определенные риски) для проверки результатов выполнения тестов.
3. Техническая документация, для понимания валидных и невалидных данных.

### Перечень и описание возможных рисков при автоматизации:

1. Отсутствие технической документации.
2. Не значительное изменение реализации веб-элементов на странице, могут привести к падению ранее написаных авто-тестов.
3. Авто-тесты не проверяют графический интерфейс (GUI) сайта.  

### Перечень необходимых специалистов для автоматизации:

Один специалист по автоматизации тестирования, который умеет работать с инструментами описанными выше.

### Интервальная оценка с учетом рисков (в часах):

Для осуществления данного тест-плана по автоматизации, ориентировочно потребуется 23 рабочих часа.