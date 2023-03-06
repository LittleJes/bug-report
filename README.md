# Примеры баг-репортов для сайта https://www.lamoda.ru/

## 1. Меняется состояние кнопки для добавления в избранное если закрыть окно авторизации

**Окружение:** YandexBrowser 23.1.3.949(64-bit), Win 10 (64), 1280x1024

**Шаги:**

Шаг 1. Открыть любую страницу где отображается товар

Шаг 2. Нажать на кнопку "Добавить в избранное"

Шаг 3. Закрыть открывшиеся окно авторизации

**Ожидаемый результат:** Кнопка для добавления в избранное не будет менять цвет

**Фактический результат:** Кнопка для добавления в избранное становится красной

**Серьезность:** Trivial

## 2. Не закрывается окно добавления отзыва при закрытии окна авторизации

**Окружение:** YandexBrowser 23.1.3.949(64-bit), Win 10 (64), 1280x1024

**Шаги:**

Шаг 1. Открыть любую страницу где отображается товар

Шаг 2. Перейти на страницу выбранного товара

Шаг 3. Открыть отзывы - оставить отзыв

Шаг 4. Закрыть открывшиеся авторизации

**Ожидаемый результат:** Окно для добавления отзыва закроется

**Фактический результат:** При закрытии окна аторизации - окно для добавления отзыва остается открытым. При этом, если попытаться оставить отзыв - появится сообщение об отсутствии интернета. Так-же это окно не закрывается нажатием на крестик

**Серьезность:** Minor

## 3. Некорректно отображаются текст на странице теста "Определите свой стиль"

**Окружение:** YandexBrowser 23.1.3.949(64-bit), Win 10 (64), 1280x1024

**Шаги:**

Шаг 1. Открыть главную страницу

Шаг 2. Нажать на раздел "Определите ваш стиль"

Шаг 3. Выбрать пол и нажать начать

**Ожидаемый результат:** Текс "Согласна/Не согласена" будет отображаться корректно по бокам от кнопок 

**Фактический результат:** Текс "Согласна/Не согласена" наезжает на кнопки теста 

**Серьезность:** Major

## 4. Не отображается включение чек-бокса в фильтрах каталога

**Окружение:** YandexBrowser 23.1.3.949(64-bit), Win 10 (64), 1280x1024

**Шаги:**

Шаг 1. Открыть любую котегорию (Например обувь)

Шаг 2. Открыть любой фильтр и включить любой чек-боксы

Шаг 3. Не нажимая применить - открыть другой фильтр и влючить любые чек-боксы

**Ожидаемый результат:** Чек-боксы у выбранных фильтров будут отображаться как влюченные

**Фактический результат:** Выбранные чек-боксы отображаются пустыми, при этом они включены 

**Серьезность:** Trivial