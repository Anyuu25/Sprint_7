# Sprint_7
Тестирование API

API-тесты для сервиса Яндекс.Самокат

Документация сервиса:
qa-scooter.praktikum-services.ru/docs/.


## Файлы:
- allure_results - каталог с отчетом о тестировании
- tests/ - каталог с автотестами
- tests/test_create_courier.py - файл с проверками создания курьера 
- tests/test_login_courier.py - файл с проверками авторизации курьера
- tests/test_order.py - файл с проверками создания заказа
- tests/test_orders_list.py - файл с проверками получения списков заказа
- endpoints.py - файл с эндпоинтами
- urls.py - файл с URL сервиса
- data.py - данные со вспомогательными данными для тестирования
- requirements.txt - файл с внешними зависимостями
- conftest.py - файл с фикстурой

Перед работой с репозиторием требуется установить зависимости 
```
pip install -r requirements.txt
```
Запустить все тесты
```
pytest tests --alluredir=allure_results
```
Посмотреть отчет о тестировании
```
allure serve allure_results
```