# Метаданные
| Поле         | Значение                 |
|--------------|--------------------------|
| Проект       | https://www.saucedemo.com|
| Версия       | v1.0|
| Автор        | Булат Камалов|
| Дата         | 14.05.2026|
| Окружение    | Mozilla Firefox 150.0(64-bit)|


| ID | Проверка | Ожидаемый результат | Статус | Баг/ Комментарий |
| --- | --- | --- | --- | --- |
| 1 | Наличие плейсхолдеров в полях | В полях отображается серый текст "Username" и "Password" | ✅ |  |
| 2 | Ввод `secret_sauce` в поле пароля | Символы скрыты точками | ✅ |  |
| 3 | Навигация с помощью нажатия `Tab` | Фокус корректно переключается с поля логина на поле пароля | ✅ |  |
| 4 | Отправка формы нажатием `Enter` | Форма отправляется так же, как при клике на кнопку `Login` | ✅ |  |
| 5 | Успешная авторизация (`standard_user` + `secret_sauce`) | Переход на страницу каталога (/inventory.html) | ✅ |  |
| 6 | Несуществующий логин (`fake_user` + `secret_sauce`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| 7 | Неверный пароль (`standard_user` + `fake_pass`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| 8 | Заблокированный аккаунт (`locked_out_user` + `secret_sauce`) | Ошибка: `Epic sadface: Sorry, this user has been locked out.` | ✅ |  |
| 9 | Пустой логин ([пусто] + `secret_sauce`) | Ошибка: `Epic sadface: Username is required` | ✅ |  |
| 10 | Пустой пароль(`standard_user` + [пусто]) | Ошибка: `Epic sadface: Password is required` | ✅ |  |
| 11 | Оба поля пустые([пусто] + [пусто]) | Ошибка: `Epic sadface: Username is required` | ✅ |  |
| 12 | Чувствительность к регистру (`STANDARD_USER` + `secret_sauce`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| 13 | Пробелы в начале и конце логина | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
