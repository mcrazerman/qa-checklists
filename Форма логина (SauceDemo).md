https://www.saucedemo.com

| # | Проверка | Ожидаемый результат | pass/fail | Комментарий |
| --- | --- | --- | --- | --- |
| 1 | Наличие плейсхолдеров в полях | В полях отображается серый текст "Username" и "Password" | pass |  |
| 2 | Ввод secret\_sauce в поле пароля | Символы скрыты точками | pass |  |
| 3 | Навигация с помощью нажатия Tab | Фокус корректно переключается с поля логина на поле пароля | pass |  |
| 4 | Отправка формы нажатием Enter | Форма отправляется так же, как при клике на кнопку "Login" | pass |  |
| 5 | Успешная авторизация (standard\_user + secret\_sauce) | Переход на страницу каталога (/inventory.html) | pass |  |
| 6 | Несуществующий логин (fake\_user + secret\_sauce) | Ошибка: "Epic sadface: Username and password do not match…" | pass |  |
| 7 | Неверный пароль (standard\_user + fake\_pass) | Ошибка: "Epic sadface: Username and password do not match…" | pass |  |
| 8 | Заблокированный аккаунт (locked\_out\_user + secret\_sauce) | Ошибка: "Epic sadface: Sorry, this user has been locked out." | pass |  |
| 9 | Пустой логин ([пусто] + secret\_sauce) | Ошибка: "Epic sadface: Username is required" | pass |  |
| 10 | Пустой пароль(standard\_user + [пусто]) | Ошибка: "Epic sadface: Password is required" | pass |  |
| 11 | Оба поля пустые([пусто] + [пусто]) | Ошибка: "Epic sadface: Username is required" | pass |  |
| 12 | Чувствительность к регистру (STANDARD\_USER + secret\_sauce) | Ошибка: "Epic sadface: Username and password do not match…" | pass |  |
| 13 | Пробелы в начале и конце логина | Ошибка: "Epic sadface: Username and password do not match…" | pass |  |
