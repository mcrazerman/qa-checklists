# Метаданные
| Поле         | Значение                 |
|--------------|--------------------------|
| Проект       | https://www.saucedemo.com|
| Версия       | v1.0|
| Автор        | Булат Камалов|
| Дата         | 14.05.2026|
| Окружение    | Linux Mint 22.2 (Zara), Mozilla Firefox 150.0(64-bit) |


| ID | Проверка | Ожидаемый результат | Статус | Баг/ Комментарий |
| --- | --- | --- | --- | --- |
| LOGIN-1 | Наличие плейсхолдеров в полях | В полях отображается серый текст "Username" и "Password" | ✅ |  |
| LOGIN-2 | Ввод `secret_sauce` в поле пароля | Символы скрыты точками | ✅ |  |
| LOGIN-3 | Навигация с помощью нажатия `Tab` | Фокус корректно переключается с поля логина на поле пароля | ✅ |  |
| LOGIN-4 | Отправка формы нажатием `Enter` | Форма отправляется так же, как при клике на кнопку `Login` | ✅ |  |
| LOGIN-5 | Успешная авторизация (`standard_user` + `secret_sauce`) | Переход на страницу каталога (/inventory.html) | ✅ |  |
| LOGIN-6 | Несуществующий логин (`fake_user` + `secret_sauce`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| LOGIN-7 | Неверный пароль (`standard_user` + `fake_pass`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| LOGIN-8 | Заблокированный аккаунт (`locked_out_user` + `secret_sauce`) | Ошибка: `Epic sadface: Sorry, this user has been locked out.` | ✅ |  |
| LOGIN-9 | Пустой логин ([пусто] + `secret_sauce`) | Ошибка: `Epic sadface: Username is required` | ✅ |  |
| LOGIN-10 | Пустой пароль(`standard_user` + [пусто]) | Ошибка: `Epic sadface: Password is required` | ✅ |  |
| LOGIN-11 | Оба поля пустые([пусто] + [пусто]) | Ошибка: `Epic sadface: Username is required` | ✅ |  |
| LOGIN-12 | Чувствительность к регистру (`STANDARD_USER` + `secret_sauce`) | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
| LOGIN-13 | Пробелы в начале и конце логина | Ошибка: `Epic sadface: Username and password do not match…` | ✅ |  |
