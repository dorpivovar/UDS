# Space-Sentinel
Проект представляет собой игру в жанре платформер
### Игровой процесс:
В игре будет несколько уровней, игрок появляется в начале уровня и его цель добраться до конца не умерев. Персонаж может стрелять, прыгать и ходить. Уровни представляют собой карту с платформами.
### Управление
* Стрелка влево - движение влево
* Стрелка вправо - движение вправо
* Z - Стрельба
* Стрелка вверх - прыжок
* Escape - главное меню
### Как запустить:
1. Скачайте проект как архив либо при помощи git clone.
2. Установите [Python 3.12](https://www.python.org/downloads/release/python-3120/) и [Pygame 2.5.2](https://github.com/pygame/pygame) (работоспособность на версиях ниже не гарантирую).
3. Запустите main.py
### Руководство программиста:
1. main.py - основной файл
    1. класс Game - основной класс игры
        1. функция show_start_screen - стартовый экран с выбором уровня
        2. функция complete_game -  экран окончания игры
        3. функция load_level - загрузка уровня
        5. функция is_dead - убивает игрока если он упал в пустоту
        6. функция kill_player - убивает игрока и очищает экран от пуль и загружает уровень заново
        7. функция run - основная функция с главным циклом игры
2. editor.py - редактор уровней
    1. класс Editor - класс редактора
        1. функция run - основная функция с главным циклом редактора
3. scripts
    1. entities.py - файл со всем что связано с сущностями
        1. класс PhysicsEntity - класс сущности
        2. класс Player - класс игрока
        3. класс Enemy - класс врагов
    2. tilemap.py
        1. класс Tilemap - все что связано с тайлами, уровнями
    3. utils.py
        1. функция load_image - загрузка изображения
        2. функция load_images - загрузка группы изображений
        3. класс Animation - класс анимаций
4. data
    1. images - изображения 
        1. entities - изображения сущностей
        2. tiles - тайлы
5. maps - файлы карт в формате json
### Заключение
Конечно я реализовал не все что хотел, убийство врагов работает очень криво и сами враги не могут убить игрока.
### Список используемой литературы
* Документация pygame 
* Учебник Яндекс лицея
* ChatGPT
* Youtube
* editor.py взят от сюда - https://youtu.be/2gABYM5M0ww?si=bWkh74S6DqLiwBZo&t=8545
