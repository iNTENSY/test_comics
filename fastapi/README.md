
### Запуск проекта
Клонируйте репозиторий и перейдите в него в командной строке
```
git clone https://github.com/iNTENSY/test_comics.git
```
```
cd .\comics\fastapi\
```
Cоздайте и активируйте виртуальное окружение
```
python3 -m venv venv # Для Linux и macOS
python -m venv venv # Для Windows
```
```
venv/Scripts/activate # Для Windows
source venv/bin/activate # Для Linux и macOS
```
Установите зависимости из файла `requirements.txt`
```
pip install -r requirements.txt
```
Создайте файл `.env`, в котором укажете свои переменные окружения <br>
(Примечание: пример `.env` файла указать в `.env_example`)

Примените миграции к вашей базе данных с помощью `alembic`
```
alembic upgrade head
```
Для запуска сервера вам потребуется запустить файл `app.py`, 
который в свою очередь находится в каталоге `src`.

***
## Полная документация к API проекта:

Перечень запросов к ресурсу можно посмотреть в описании API

```
http://127.0.0.1:8000/docs/
http://127.0.0.1:8000/redoc/
```