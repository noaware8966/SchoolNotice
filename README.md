1.4. Во время установки поставьте галочку Add Python to PATH
2. Установка виртуального окружения
2.1. Создаём папку Django и внутри неё папку djsite
C:\Python\django\djsite
2.2. Откройте командную строку (Cmd) и перейдите в каталог, где хотите создать проект, выполнять поочередно:
cd \
cd Python/django/djsite
2.3. Создайте виртуальное окружение:
python -m venv venv
2.4. Активируйте виртуальное окружение:
venv\Scripts\activate
2.5. Результат
2.6. Закрываем Cmd
3. Установка Django
3.1. Открываем PyCharm
3.2. Загружаем папку djsite в PyCharm (File → Open → выбираем djsite)
3.3. Открываем встроенный терминал PyCharm (Левый нижний угол)
3.4. В терминале выполняем следующую команду: 
pip install django
3.5.  Ждём сообщения об успешной установке
4. Создание проекта
4.1. Запустите команду:
django-admin startproject hotel
4.2. Перейдите в папку проекта
cd hotel
5. Создание приложения
5.1. Запустите команду:
python manage.py startapp dbms
5.2. Регистрация dbms в Django
5.3. Откройте hotel/settings.py и в INSTALLED_APPS добавьте в список INSTALLED_APPS элемент ‘dbms’:
