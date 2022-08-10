# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.
Альтернативная команда *git commit -am "<сообение к комиту"*. Исользуется в случае когда файл уже закомичен.   
<https://github.com/>

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
## Помещение текущих изменений в отдельное хранилище, возврат к исходному состоянию
Команда git stash предназначена для того, чтобы поместить текущие изменения в отдельное хранилище и вернуть файлы к исходному состоянию. То есть git stash прячет изменения в файлах и сохраняет эти изменения отдельно, чтобы потом можно было их вернуть.

## Помещаем ненужные файлы в .gitignore
для того чтобы Git не показывал ненужные файлы как неотслеживаемые создается файл  *.gitignore*. Там прописываем файлы которые _Git_ будет игнорировать.

## Команда **_git log --graph_**
Позволяет просмотреть журнал изменений с учетом создания и изменений в  ветках, с отображением __слияний и переходов__
=======
## Бесконфликтное слияние.
Вроде как если слияние веток прошло без конфликта то можно не комитить

