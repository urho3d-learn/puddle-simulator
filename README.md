# Симулятор лужи

Лицензия на код: Public Domain.

В папке [result](result) есть скомпилированная версия игры.

Цель игры - окрасить всю жидкость в один цвет за определенное число ходов. Остаток ходов отображается в левом
верхнем углу экрана. Цвета выбираются с помощью столбца кнопок на правой стороне экрана. При успешном прохождении уровня,
открывается доступ к следующему. Перемещаться между открытыми уровнями можно с помощью кнопок,
расположенных в левом нижнем углу.

Прохождение первого уровня: выберите синий цвет и щелкните по желтому участку лужи.

Видео: https://www.youtube.com/watch?v=TUX3NBUSC4o

![Screenshot](images/play.png)

## Редактирование уровней

Существует секретная кнопка E, которая включает режим редактирования. В этом режиме
фон окрасится в красный цвет, а также появится белый круг, показывающий границы сосуда.
В левом верхнем углу экрана станут доступны кнопки для изменения числа ходов.

![Screenshot](images/editor.png)

Чтобы изменить размер ёмкости, нужно зажать клавишу SHIFT и двигать мышку.
Левой кнопкой мыши можно создать молекулу выбранного цвета. Клавиша ПРОБЕЛ
создает сразу 5 молекул в случайных местах. Таким способом удобно быстро заполнить ёмкость.
Удерживая правую кнопку мыши можно менять цвет уже существующих молекул.
Чтобы сохранить изменения в файл, нажмите клавишу S. Если вам нужно откатить
изменения, вы можете использовать кнопку перезапуска, чтобы перезагрузить
уровень из файла. Чтобы выйти из режима редактирования, вновь нажмите E.

Видео: https://www.youtube.com/watch?v=uGWimUDtxpE

Помните! Плотность молекул должна быть высокой, чтобы заливка работала.

Совет: перед самым сохранением вы можете добавить какую-то молекулу,
чтобы уровень стартовал с колеблющейся жидкостью.

## Создание новых уровней

Список уровней хранится в текстовом файле GameData/Levels.txt.
Просто добавьте туда новую строку с именем уровня. После изменения этого файла
обязательно перезапускайте игру, так как список уровней считывается только при
запуске игры. Сами файлы уровней находятся в папке GameData/Scenes.
Если в списке GameData/Levels.txt есть какой-то уровень, но его файл отсутствует
в папке GameData/Scenes, то игра создаст пустой уровень, и вы можете его
отредактировать и сохранить. Вы можете даже удалить все файлы из папки
GameData/Scenes и создать собственный набор уровней.

Внимание! Не оставляйте пустых строк в файле GameData/Levels.txt.

## Сброс прогресса

Удалите файл `c:\Users\ИМЯ_ПОЛЬЗОВАТЕЛЯ\AppData\Roaming\1vanK\PuddleSimulator\Config.xml`.

*Старая версия игры: <https://github.com/1vanK/PuddleSimulator>.*
