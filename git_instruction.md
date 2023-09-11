# Инструкция по работе с системой контроля версий Git

## Что такое git
><span style="color:green">Git - это одна из самых популярных реализаций систем контроля версий.

### Основные команды

* <span style="color:red">**git init**

><span style="color:green">Создает репозиторий в выбранной папке

* <span style="color:red">**git status**
><span style="color:green">Команда для просмотра состояния репозитория, есть ли изменения или нет

* <span style="color:red">**git add**
><span style="color:green">Команда для добавления изменений

* <span style="color:red">**git commit -m "new message"**
><span style="color:green">Команда для добавления комментария к сохраненным изменениям

* <span style="color:red">**git log**
><span style="color:green">Команда для просмотра истории коммитов

* <span style="color:red">**git checkout**
><span style="color:green">Команда для переключения между коммитами

* <span style="color:red">**git diff**
><span style="color:green">Команда которая показывает не добавленные изменения


### Команды второго семинара

><span style="color:green">Чтобы добавить картинку в файл, нужно написать следующую команду:

![branch](branch.png)

><span style="color:green">Чтобы git игнорировал файлы или папки, их нужно добавить в файл .gitignore

* <span style="color:red">**git branch**
><span style="color:green">Команда git для управления ветками

* <span style="color:red">**git branch branch_name**
><span style="color:green">Команда для создания новой ветки

* <span style="color:red">**git checkout branch_name**
><span style="color:green">Команда для переключения между ветками

* <span style="color:red">**git merge branch_name**
><span style="color:green">Команда для слияния веток

* <span style="color:red">**git branch -d branch_name**
><span style="color:green">Команда для удаления ветки


><span style="color:green">Иногда при слиянии веток происходит конфликт изменений

![conflict](conflict.png)

><span style="color:green">Git предлагает несколько решений:

* <span style="color:red">**Accept Current Change**
><span style="color:green">Принять только изменения текущей ветки

* <span style="color:red">**Accept Incoming Change**
><span style="color:green">Принять только изменения входящей ветки

* <span style="color:red">**Accept Both Changes**
><span style="color:green">Принять изменения обоих веток

* <span style="color:red">**Compare Changes**
><span style="color:green">Сравнить изменения в ветках

* <span style="color:red">**git branch -D branch_name**
><span style="color:green">Команда для удаления ветки c несохраненными изменениями

* <span style="color:red">**git log --graph**
><span style="color:green">Команда которая показывает в терминале графическое представление веток

### Команды по работе с удалённым репозиторием

* <span style="color:red">**git clone**
><span style="color:green">Команда для копирования существующего удаленного репозитория

* <span style="color:red">**git pull**
><span style="color:green">Команда для загрузки содержимого из удаленного репозитория и слияния его с локальным репозиторием

* <span style="color:red">**git push**
><span style="color:green">Команда для выгрузки содержимого из локального репозитория в удаленный репозиторий

* <span style="color:red">**GitHub**
><span style="color:green">Это один из сервисов для работы с удаленными репозиториями

* <span style="color:red">**Fork**
><span style="color:green">Функция на GitHub которая позволяет создать копию чужого репозитория на наш аккаунт GitHub и проводить любые изменения не затрагивая оригинальный репозиторий

* <span style="color:red">**Pull request**
><span style="color:green">Это предложение изменений или поправок кода чужому репозиторию, который мы ранее скопировали с помощью Fork

