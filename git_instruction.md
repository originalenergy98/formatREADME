# Подготовка репозиторя
*Перед началом работы нужно представиться репозиторию:*
* git config user.name 
* git config user.email

*Можно прописать name и email локально:*
* git config --local user.name 
* git config --local user.email

*После нужно создать локальный репозиторий:*
* git init

# Создание "сохранений" 
*Для того, чтобы сохранить наши изменения, нужно добавить их через команду add*

* git add file_name

    Добавит к отслеживанию файл с именем file_name

* git add .

    Добавит все файлы

*После того, как добавили файлы для отслеживания, нужно зафиксировать их изменения:*
* git commit -m "commit info"

*Если файл был внесен с помощью команды add хотя бы один раз, то можно дальше просто использовать:*

* git commit -a -m "commit info"


# Проверока состояния репозитория
*Для отслеживания состояния репозитория существует много команд:*
* git status

    Показывает незакомиченные изменения
    
* git log

    Показывает историю изменений

* git diff

    Показывает разницу между текущими изменениями и теми что уже закомичены

* git diff branch_name

    Показывает разницу между текущими изменениями и в ветке branch_name 

* git show

    Показывает изменения для последнего комита

* git show commit_tag

    Показывает изменения внесенные в этом комите с тегом commit_tag

# Перемещение между сохранениями (обязательно про возврат в конце на конец ветки master")
Команды:
* git checkout commit_tag

    Позваляет перейти к изменениям в коммите с тегом commit_tag
* git ccheckout master

    Вернет вас к актуальному состоянию (перейдет в ветку master)

# Журнал изменений (git log)
*Показывает историю комитов:*
* git log

* git log --graph
    Показывает визуальную историю веток


# Ветки в git
*Команды для работы с ветками:*
* git branch

    Показывают все ветки
* git branch branch_name

    Создает новую ветку с именем branch_name

* git checkout branch_name

    Перемещает на ветку branch_name

# Слияние веток и решение конфликтов
* git merge branch_name

    Позваляет влить ветку branch_name в текущую

*В случае возникновения конфликта нужно вручную исправить не совподающие изменения и сделать комит с этим конфликтом*


# Удаление веток

* git branch -d branch_name

    Удаляет ветку с именем branch_name

# Работа с удаленными репозиториями 

* git clone (адрес репозитория)
    Позваляет склонировать внешние репозиторий на ПК

* git pull
    Позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией

* git push
    Позваляет отправить нашу версию репозиторияна на внешний репозиторий. Требуется авторизация на внешним репозитории.