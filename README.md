<h1 align="center">Звіт з лабораторної роботи №2</h1>
<h2 align="center">Знайомство з Docker</h2>
 
Запуск першого Docker-контейнера. Команда docker run -d -p 8080:80 docker/welcome-to-docker завантажує та запускає образ welcome-to-docker. Ми бачимо, як Docker завантажує необхідні шари з репозиторію Docker Hub.
<p align="center">
<img src="Screenshots/ (1).png" alt="(1)"/>
</p>
Підтвердження успішного запуску контейнера. Вітальна сторінка показує вітальне повідомлення, яке підтверджує, що ви успішно запустили свій перший контейнер. Сторінка містить опції для поширення в соціальних мережах та святковий анімований конфетті.
<p align="center">
<img src="Screenshots/ (2).png" alt="(2)"/>
</p>
Інтерфейс Docker Desktop для керування контейнерами. Панель керування показує використання ресурсів працюючого контейнера, включаючи використання CPU (0.00% / 1200%) та пам'яті (9.45MB / 5.37GB). Контейнер з назвою "keen_keldysh" працює на порту 8080:80.
<p align="center">
<img src="Screenshots/ (3).png" alt="(3)"/>
</p>
Перевірка файлової системи контейнера. Використовуючи термінальний інтерфейс Docker Desktop, ми можемо побачити внутрішню структуру файлів контейнера за допомогою команди ls -la, яка показує різні системні директорії та їх права доступу.
<p align="center">
<img src="Screenshots/ (4).png" alt="(4)"/>
</p>
Деталі конфігурації контейнера. Вкладка inspect показує конфігурацію контейнера у форматі JSON, включаючи змінні середовища, версію nginx (1.25.3) та команди контейнера. Це надає детальну інформацію про те, як налаштований та працює контейнер.
<p align="center">
<img src="Screenshots/ (5).png" alt="(5)"/>
</p>

# Лабораторна робота: Розробка Todo App з Docker

Клонування репозиторію з прикладом Todo застосунку. Використовуємо команду `git clone` для завантаження початкового коду з GitHub репозиторію docker/getting-started-todo-app.

<p align="center">
<img src="Screenshots/ (6).png" alt="(6)"/>
</p>

Запуск Docker Compose для збірки та розгортання додатку. Команда `docker compose watch` автоматично збирає та запускає всі необхідні контейнери для роботи застосунку: клієнт, бекенд, базу даних MySQL та phpMyAdmin.

<p align="center">
<img src="Screenshots/ (7).png" alt="(7)"/>
</p>

Перевірка работи Todo застосунку через веб-браузер. Після успішного запуску всіх контейнерів, застосунок доступний за адресою localhost. На головній сторінці бачимо привітання "Hello world!" та форму для додавання нових завдань.

<p align="center">
<img src="Screenshots/ (8).png" alt="(8)"/>
</p>

Структура файлів бекенд частини. У директорії routes знаходяться JavaScript файли, що відповідають за різні функції застосунку: додавання, видалення, оновлення та отримання списку завдань.

<p align="center">
<img src="Screenshots/ (9).png" alt="(9)"/>
</p>

Приклад коду серверної частини. Файл getGreeting.js містить масив привітань та функцію, яка випадковим чином вибирає одне з них для відображення на головній сторінці.

<p align="center">
<img src="Screenshots/ (10).png" alt="(10)"/>
</p>

Перевірка роботи випадкових привітань. На головній сторінці додатку відображається привітання "Whalecome!", яке обирається випадковим чином з масиву можливих варіантів.

<p align="center">
<img src="Screenshots/ (11).png" alt="(11)"/>
</p>

Оновлення привітання при перезавантаженні сторінки. При оновленні сторінки бачимо нове випадкове привітання "All hands on deck!".

<p align="center">
<img src="Screenshots/ (12).png" alt="(12)"/>
</p>

Ще один приклад випадкового привітання. Після чергового перезавантаження відображається привітання "Charting the course ahead!".

<p align="center">
<img src="Screenshots/ (13).png" alt="(13)"/>
</p>

Структура клієнтської частини додатку. В директорії components містяться React компоненти, що відповідають за різні елементи інтерфейсу користувача.

<p align="center">
<img src="Screenshots/ (14).png" alt="(14)"/>
</p>

Код компонента форми додавання нового завдання. Файл AddNewItemForm.jsx містить React компонент з полем введення та обробкою події додавання нового завдання.

<p align="center">
<img src="Screenshots/ (15).png" alt="(15)"/>
</p>

Інтерфейс додавання нового завдання. У поле введення можна ввести текст завдання, яке потрібно додати до списку.

<p align="center">
<img src="Screenshots/ (16).png" alt="(16)"/>
</p>

Структура клієнтської частини додатку. Директорія src містить основні файли React додатку - компоненти, стилі та точку входу.

<p align="center">
<img src="Screenshots/ (17).png" alt="(17)"/>
</p>

Стилізація додатку. Файл index.scss містить базові стилі, включаючи імпорт Bootstrap, налаштування кольору фону та шрифту.

<p align="center">
<img src="Screenshots/ (18).png" alt="(18)"/>
</p>

Перевірка стилізації. На сторінці додатку бачимо застосування заданих стилів - світло-блакитний фон та шрифт Lato.

<p align="center">
<img src="Screenshots/ (19).png" alt="(19)"/>
</p>

Головна сторінка Docker Hub. Платформа надає доступ до найбільшої бібліотеки контейнерних образів та інструменти для роботи з Docker.

<p align="center">
<img src="Screenshots/ (20).png" alt="(20)"/>
</p>

markdownCopy# Лабораторна робота: Розробка Todo App з Docker 

Створення репозиторію на Docker Hub. Заповнюємо необхідні поля для створення нового репозиторію: назва простору імен, назва репозиторію та налаштування видимості.

<p align="center">
<img src="Screenshots/ (21).png" alt="(21)"/>
</p>

Налаштування створеного репозиторію. Після створення отримуємо доступ до налаштувань репозиторію та інструкцій щодо завантаження образів.

<p align="center">
<img src="Screenshots/ (22).png" alt="(22)"/>
</p>

Збірка Docker образу. Використовуємо команду docker build для створення образу нашого додатку, спостерігаємо за процесом збірки та копіювання необхідних файлів.

<p align="center">
<img src="Screenshots/ (23).png" alt="(23)"/>
</p>

Завантаження образу на Docker Hub. За допомогою команди docker push завантажуємо створений образ у наш репозиторій на Docker Hub.

<p align="center">
<img src="Screenshots/ (24).png" alt="(24)"/>
</p>
