Внизу приведен пример работы программы!
==================================
Более подробно узнать о работе пакета можно в разделе wiki "[group_queue](https://github.com/AppLoidx/lilly-chan/wiki/group_queue)"<br><br>
Краткий курс:

        history.py - для записи истории
        queue.py - для работы с очередью
        person.py - класс объекта в очереди
        
Мне лень (по крайней мере сейчас) писать документацию на этот говнокод. Так что кто хочет разбирайтесь сами.
Единственное, что скажу, так это то что внутри queque.py использован класс Date из основного проекта. Поэтому если хотите запустить
этот проект на свой комп и поиграться, то
        
        1. Либо удалите все используемые date.get_time(), не забыв удалить импорт.
        
        2. Либо в ручную поставить рядом Date и импортировать его. Есои поставите в ту же папку, то импорт примерно будет таким:
                
                from date import Date

                date = Date()

                print(date.Date()) # Выведет текущее время.

        3. Либо скачать весь проект ( там еще больше говнокода)
        
        P.S. Также обязательно нужно переопределить self._set_group_list(), а именно изменить путь к файлу со списком группы.
             Класс Date - работает только с интернетом, так как получает дату со стороннего сайта. Его реализация есть в parser

Если вас заинтересует, то можно еще посмотреть пакеты questions - вопросы по теме Java; schedule - расписание (лишь для P3112)

add_person и delete_person использует номер ИСУ как идентификационный номер.

**ПРИМЕР РАБОТЫ ПРОГРАММЫ**

(В скобках указан номер ИСУ)

======================
1. Сидорова Алина (23)
2. Тарасов Александр (24)
3. Хлюстов Илья (25)
4. Шайхатаров Артур (26)
5. Шаяхметов Ислам (27)
6. Алексеев Андрей (1)
7. Анищенко Анатолий (2)
8. Атикеев Роман (3)
9. Барышев Вадим (4)
10. Буланов Кирилл (5)
11. Гараева Рамина (6)
12. Гогидзе Полина (7)
13. Гурин Евгений (8)
14. Давидович Даниил (9)
15. Емельянов Григорий (10)
16. Ефаринов Павел (11)
17. Забирова Евгения (12)
18. Иванов Илья (13)
19. Колоколов Артём (14)
20. Кульбако Артемий (15)
21. Куприянов Артур (16)
22. Лозовцов Владислав (17)
23. Максимов Александр (18)
24. Мосягин Иван (19)
25. Носов Михаил (20)
26. Очаковский Сергей (21)
27. Рождественский Никита (22)

queue.delete_position('13')
=================================================
1. Сидорова Алина (23)
2. Тарасов Александр (24)
3. Хлюстов Илья (25)
4. Шайхатаров Артур (26)
5. Шаяхметов Ислам (27)
6. Алексеев Андрей (1)
7. Анищенко Анатолий (2)
8. Атикеев Роман (3)
9. Барышев Вадим (4)
10. Буланов Кирилл (5)
11. Гараева Рамина (6)
12. Гогидзе Полина (7)
13. Гурин Евгений (8)
14. Давидович Даниил (9)
15. Емельянов Григорий (10)
16. Ефаринов Павел (11)
17. Забирова Евгения (12)
18. Колоколов Артём (14)
19. Кульбако Артемий (15)
20. Куприянов Артур (16)
21. Лозовцов Владислав (17)
22. Максимов Александр (18)
23. Мосягин Иван (19)
24. Носов Михаил (20)
25. Очаковский Сергей (21)
26. Рождественский Никита (22)

queue.add_person('13', 4)
=================================================
1. Сидорова Алина (23)
2. Тарасов Александр (24)
3. Хлюстов Илья (25)
4. Иванов Илья (13)
5. Шайхатаров Артур (26)
6. Шаяхметов Ислам (27)
7. Алексеев Андрей (1)
8. Анищенко Анатолий (2)
9. Атикеев Роман (3)
10. Барышев Вадим (4)
11. Буланов Кирилл (5)
12. Гараева Рамина (6)
13. Гогидзе Полина (7)
14. Гурин Евгений (8)
15. Давидович Даниил (9)
16. Емельянов Григорий (10)
17. Ефаринов Павел (11)
18. Забирова Евгения (12)
19. Колоколов Артём (14)
20. Кульбако Артемий (15)
21. Куприянов Артур (16)
22. Лозовцов Владислав (17)
23. Максимов Александр (18)
24. Мосягин Иван (19)
25. Носов Михаил (20)
26. Очаковский Сергей (21)
27. Рождественский Никита (22)

queue.swap('5', '7')
=================================================
1. Сидорова Алина (23)
2. Тарасов Александр (24)
3. Хлюстов Илья (25)
4. Иванов Илья (13)
5. Шайхатаров Артур (26)
6. Шаяхметов Ислам (27)
7. Алексеев Андрей (1)
8. Анищенко Анатолий (2)
9. Атикеев Роман (3)
10. Барышев Вадим (4)
11. Гогидзе Полина (7)
12. Гараева Рамина (6)
13. Буланов Кирилл (5)
14. Гурин Евгений (8)
15. Давидович Даниил (9)
16. Емельянов Григорий (10)
17. Ефаринов Павел (11)
18. Забирова Евгения (12)
19. Колоколов Артём (14)
20. Кульбако Артемий (15)
21. Куприянов Артур (16)
22. Лозовцов Владислав (17)
23. Максимов Александр (18)
24. Мосягин Иван (19)
25. Носов Михаил (20)
26. Очаковский Сергей (21)
27. Рождественский Никита (22)

queue.swap('12','5')
=================================================
1. Сидорова Алина (23)
2. Тарасов Александр (24)
3. Хлюстов Илья (25)
4. Иванов Илья (13)
5. Шайхатаров Артур (26)
6. Шаяхметов Ислам (27)
7. Алексеев Андрей (1)
8. Анищенко Анатолий (2)
9. Атикеев Роман (3)
10. Барышев Вадим (4)
11. Гогидзе Полина (7)
12. Гараева Рамина (6)
13. Забирова Евгения (12)
14. Гурин Евгений (8)
15. Давидович Даниил (9)
16. Емельянов Григорий (10)
17. Ефаринов Павел (11)
18. Буланов Кирилл (5)
19. Колоколов Артём (14)
20. Кульбако Артемий (15)
21. Куприянов Артур (16)
22. Лозовцов Владислав (17)
23. Максимов Александр (18)
24. Мосягин Иван (19)
25. Носов Михаил (20)
26. Очаковский Сергей (21)
27. Рождественский Никита (22)

HISTORY
===========================

Создана новая очередь

Колоколов Артём удален из очереди в 3:34:59

В позицию 4 добавлен Иванов Илья в 3:34:59

Поменялись местами: Гогидзе Полина <-> Буланов Кирилл в 3:34:59

Поменялись местами: Буланов Кирилл <-> Забирова Евгения в 3:34:59


Это самая простая реализация для тестирования и примера. Весь класс устроен так, что вызовы методов лишь возвращают значения, поэтому
его легко можно ставить в другой код. Потом я что нибудь сделаю с импортом Date.
