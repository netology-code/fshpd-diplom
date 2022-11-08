# Дипломный проект профессии «Разработка на Python. Базовый курс»

## EnglishCard

### Цель проекта

Цель проекта - разработать Telegram-бот для изучения английского языка. Бот будет предлагать различные варианты слов и проверять их правильный перевод.

Вам предстоит:
- разработать программу-бота на Python
- спроектировать и реализовать базу данных (БД) для программы
- настроить взаимодействие бота с Yandex API
- написать документацию по использованию программы.

В результате выполнения этого задания вы:
- получите практический опыт работы с Telegram и Yandex API
- закрепите навыки работы с GitHub и программирования на языке Python
- разработаете с нуля полноценный программный продукт, который можно будет добавить в портфолио разработчика.

------

### Чеклист готовности к работе над проектом

1. У вас должен быть установлен Python 3.9/3.10 и любая IDE. Мы рекомендуем работать с Pycharm.
2. Настроен компьютер для работы с БД PostgreSQL.
3. Установлен git и создан аккаунт на Github.
4. Cоздан бот в Telegram:
- инструкцию по созданию бота можно посмотреть [здесь](https://lifehacker.ru/kak-sozdat-bota-v-telegram/)
- за основу бота можно взять код из модуля [main.py](https://github.com/netology-code/fshpd-diplom/blob/main/main.py).

Если все этапы чеклиста пройдены, то можете стартовать работу над проектом. Успехов в работе!

------

### Инструменты/ дополнительные материалы, которые пригодятся для выполнения задания

1. [Python](https://www.python.org/) + IDE([Pycharm](https://www.jetbrains.com/ru-ru/pycharm/download))
2. [Git](https://git-scm.com/) + [Github](https://github.com/)
3. [Postgre](https://www.postgresql.org/) + [PgAdmin](https://www.pgadmin.org/)
4. [Статья](https://habr.com/ru/post/580408/) по разработке бота в Telegram
5. [Инструкция](https://lifehacker.ru/kak-sozdat-bota-v-telegram/) по созданию бота в Telegram
6. Основа бота - код из модуля [main.py](https://github.com/netology-code/fshpd-diplom/blob/main/main.py)

------

### Инструкция к работе над проектом

Необходимо разработать программу-бота, которая должна выполнять следующие действия:  
1. Заполнить базу данных общим набором слов для всех пользователей (цвета, местоимения и т.д.). Достаточно 10 слов.
1. Спрашивать перевод слова, предлагая 4 варианта ответа на английском языке в виде кнопок.
2. При правильном ответе подтверждать ответ, при неправильном - предлагать попробовать снова.
3. У каждого слова должен быть пример использования. Пример использования получать из сервиса [Yandex Dictionary](https://yandex.ru/dev/dictionary/doc/dg/concepts/About.html) из блока `[ex][text]`.
4. Должна быть реализована функция добавления нового слова.
5. После добавления нового слова выводить сколько слов изучает пользователь.
6. Новые слова не должны появляться у других пользователей.
7. Должна быть реализована функция удаления слова.
8. Удаление должно быть реальзовано персонально для пользователя.
9. Работа с ботом после запуска должна начинаться с приветственного сообщения. 
<details>
  <summary>Вот пример такого сообщения</summary>
  Привет 👋
  Давай попрактикуемся в английском языке. Тренировки можешь проходить в удобном для себя темпе. 

  Причём у тебя есть возможность использовать тренажёр как конструктор и собирать свою собственную базу для обучения. Для этого воспрользуйся инструментами Добавить слово➕ или Удалить слово🔙.

  Ну что, начнём ⬇️
</details>

В качестве примера интерфейса бота можете воспользоваться следующим референсом:

<div align="center">
  <img src="https://github.com/netology-code/fshpd-diplom/blob/main/Screenshot.png" width="400" alt="Примерный дизайн бота"/>
  <p>возможный интерфейс бота</p>
</div>

-----
  
### Дополнительные требования к проекту (необязательные для получения зачёта):  

1. Реализовать категории слов (страны, средства передвижения и т.д.).
2. Не повторять изученные слова.
3. Реализовать «изученность» слова. Слово считается изученным, если его угадали 5 раз без ошибок.
4. Реализовать напоминания раз в день изучение английского языка.

------

### Правила сдачи работы

- разработан бот и все части кода объединены в главной ветке (master/main);
- в личном кабинете необходимо отправить ссылку на репозиторий с решением.

------

### Критерии оценки

Зачёт по разработанному проекту может быть получен, если созданный программный продукт соответствует следующим критериям:

1. Отсутствуют ошибки (traceback) во время выполнения программы.
2. Результат программы записывается в БД. Количество таблиц должно быть не меньше трёх. Приложена схема БД.
3. Программа добавляет новые слова в БД для каждого пользователя.
4. Программа декомпозирована на функции/классы/модули/пакеты.
5. Написана документация по использованию программы.
6. Код программы удовлетворяет PEP8. Перед отправкой решения на проверку проверьте код с помощью линтеров.
