## beckend for uaweb
### Комментарии
* При переходе по ссылке "каталог" (без выбора конкретной категории), открывается страница для первой категории
* При переходе в определенную категорию, отображаются все товары для этой категории (с пагинацией)
* Сортировка товаров не работает (верстка без селект элемента)
* Фильтр по производителю не работает (не использовал JS)
* Кнопка "Читате ще" для описания товара не работает (её лучше делать на клиенте без дополнительных запросов), для примера сделал такую кнопку в блоге и новостях, хотя на клиенте было бы лучше :)
* Для рекламных банеров много темплейтов, так что вставляем готовые в случайном порядке (пока без модели БД для рекламы и кастомных темплейтов).
* Для подписки не отображаются ошибки при неверно введенных данных (верстка), при правильно заполненых данных выскочит алерт
* Функционал по регистрации пользоватлей не добавлял (есть только администратор :)
* Не реализовано загрузку картинок для производителя и товара
* Не реализовано функционала для перебора цветов товара
* Перевод и поиск не успел сделать :(

### Запуск проекта
* Python 3 required
* `git clone` https://github.com/komarovf/beckend.git
* `cd beckend`
* Create virtual env: `python venv -m flask`
* `flask/bin/pip install -r requirements.txt`  (`flask\Scripts\pip` for Win)
* `./db_create.py` (`flask\Scripts\python db_create.py` for Win)
* `./run.py` (`flask\Scripts\python run.py`)
* Go to http://127.0.0.1:5000
* Amin page: http://127.0.0.1:5000/admin (login:pass - admin:admin)

### TODOs:
* Сделать всю инициализацию в одном месте
* Поубирать лишние импорты и комментарии из кода
* Поправить вид админ-панели до логина
* Допиливать функционал..
