# Инструкция по работе с GIT
## Lesson 1
## подготовка репозитория
Для создания репозитория необходимо выполнить команду "git init" 

## Создание коммитов
### Git add
Для добавления изменений в коммит использовать команду "git add" + <**имя файла**>

### Просмотр статуса репозитория
Для того, чтобы посмотреть состояние репозитория используется команда "git status". Для этого необходимо в папке с репозиторием написатт "git status" и Вы увидите были ли изменения в файлах, или их не было

### Создание коммитов
Для того, что бы создать коммит необходимо выполнить команду "git commit". Необходимо ввести команду "git commit-m <**текст изменения**>"


## Работа с логами и  коммитами

### Просмотр лога коммитов репозитария
Для того, что бы посмотреть все коммиты по репозиторию Необходимо ввести команду "git log". После этого вы увидете историю всех коммитов с их хеш-кодом

### Переход между коммитами
Для того, что бы перейти от одного коммита к другому необходимо ввести команду "git log", далее взять 4 символа хеш кода из нужного коммита и ввести команду "git checkout + <**4 символа хеш-кода**>"

### Переход к актуальному состоянию
Для того, что бы перейти от актуальному состоянию необходимо ввести команду "git checkout master". 

## Работа с файлом

### Просмотр разницы между текущим файлом и закоммиченным файлом
Для того, что бы просмотреть разницу между текущим файлом и закоммиченным файломнеобходимо ввести команду "git diff". 

## Lesson 2

Для создания репозитория необходимо выполнить команду "git init" 

### Просмотр статуса репозитория
Для того, чтобы посмотреть состояние репозитория используется команда "git status". Для этого необходимо в папке с репозиторием написатт "git status" и Вы увидите были ли изменения в файлах, или их не было
### Git branch
Команда которая выводит ветки


## Lesson 3

## Работа с удаленным Git
### Как подключиться к удаленному репозитарию?


Для загрузки данных в удаленный репозитарию сначала нужно к нему подключиться. В нашем примере мы используем адрес https://github.com/..../....

Для того, чтобы связать созданный нами локальный репозитарий с удаленным, выполним такую команду:


### Как отправить изменения в удаленный репозитарий?

Теперь, когда у нас в локальном репозитарии создан коммит и мы подключились к удаленному, можем отправить его на сервер. Мы это будем делать каждый раз, когда хотим обновить данные в удаленном репозитарии.

Отправка коммита осуществляется с помощью команды push, которая имеет два параметра - имя удаленного репозитория (в нашем случае origin) и ветку, в которую необходимо внести изменения (master — это ветка по умолчанию для всех репозиториев).

Если мы все сделали правильно, то отправленный файл  на удаленном сервере мы можем увидеть с помощью браузера. Важный момент – некоторые сервисы для отправки изменений могут требовать дополнительной аутентификации.

### Как клонировать удаленный репозитарий?

Если у других пользователей возникла необходимость клонировать удаленный репозитарий, они могут получить полностью работоспособную копию при помощи команды clone:

 git clone 

GitHub автоматически создаст новый локальный репозитарий в виде удаленного на собственном сервере.

### Как запросить изменения с удаленного репозитария?

В случае, если другим пользователям нет необходимости делать клон удаленного репозитария, а нужно просто получить информацию об изменениях, это можно сделать с помощью команды pull:

git pull origin master

Она скачивает новые изменения. Так как мы ничего нового не вносили с тех пор, как клонировали проект, изменений, доступных к скачиванию, нет.

