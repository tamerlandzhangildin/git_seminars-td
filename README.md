# git_seminars
# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
![Локальный контроль версий](local.png)

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.
Например, как это показано на схеме:
![Жизненный цикл файлов](lifecycle.jpeg)



### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*
1. Перейти в директорию уровнем выше: cd ..
2. Перейти в директорию двумя уровнями выше: cd ../..
3. Перейти в домашнюю директорию вашего пользователя: cd
4. Перейти в домашнюю директорию пользователя user_name: cd ~user_name
5. Перейти в директорию, в которой находились до перехода в текущую директорию: cd -

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

>Примечание. Для ещё более подробного напоминания, 
что же именно вы поменяли, можете передать аргумент -v в команду git commit. 
Это приведёт к тому, что в комментарий будет также помещена дельта/diff изменений, 
таким образом вы сможете точно увидеть все изменения которые вы совершили.

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"


 ## Для правки исползовались следующие сайты :
  [Контроль версий](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%9E-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B5-%D0%BA%D0%BE%D0%BD%D1%82%D1%80%D0%BE%D0%BB%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B9)

[Навигация](https://linuxrussia.com/terminal-navigation.html#:~:text=%D0%94%D0%BB%D1%8F%20%D0%BD%D0%B0%D0%B2%D0%B8%D0%B3%D0%B0%D1%86%D0%B8%D0%B8%20%D0%B2%20%D1%82%D0%B5%D1%80%D0%BC%D0%B8%D0%BD%D0%B0%D0%BB%D0%B5%20%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B5%D1%82%D1%81%D1%8F,%D0%B7%D0%B0%D1%82%D0%B5%D0%BC%20%D0%BF%D1%83%D1%82%D1%8C%2C%20%D0%BA%D1%83%D0%B4%D0%B0%20%D0%BD%D1%83%D0%B6%D0%BD%D0%BE%20%D0%BF%D0%B5%D1%80%D0%B5%D0%B9%D1%82%D0%B8.)

## Работа с удаленным репозиторием
1. Зарегистрироваться на  GitHub/
2. git push - внесение изменений в удаленный репозиторий. Создаем локалтный репозитроий у себя на компе, вносим изменения, набираем команду, отправляем на удаленный .
3. git pul - скачивание и слияние файлов (веток) .
4. git clone - клонирование удаленного репозитория у себя на компьютере.
5. git remote - список удаленных репозиториев.
6. Fork - создание собственных ветвлений пректа и внесение туда изменений 
![Кнопка «Создать ответвление» («Fork»)](forkbutton.png)
7. Pull request -поделится репозитарием с другим пользовмтелем.