# Инструкция по Git

## Что такое Git?

*Это - распределённая система управления версиями.*


### основные команды по работе с ветками GIT


* git status

**Команда git status отображает состояние рабочего каталога и раздела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git. Информация об истории коммитов проекта не отображается при выводе данных о состоянии. Для этого используется команда git log.**

* git branch 

*Позволяет узнать текущие существующие ветки (если добавить к "git branch" любую надпись, то будет создана новая ветка с таким названием)прим. git branch textwork - будет создана ветка textwork на которую можно перейти с помощью команды: "git checkout textwork".*

* git checkout

*Позволяет перемещаться по веткам которые были созданы и обратно на главную ветку прим. "git checkout master" - переходит на главную ветку.*

### Связанные команды git

* git tag

**Теги — это ссылки, указывающие на определенные точки в истории Git. Команда git tag обычно используется для захвата некой точки в истории, которая используется для релиза нумерованной версии (например, v1.0.1).**
*Эта команда нужна для создания репозитория* 
*(дополнение: Команда git init создает новый репозиторий Git. С ее помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий.)*


* git blame

**Общее назначение git blame — отображение метаданных автора, связанных со строками, которые были внесены в файл при коммите. Таким образом можно проследить историю кода и выяснить, какой именно код был внесен в репозиторий, как это было сделано и по какой причине.**

* git log

**Команда git log отображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также проводить поиск по ней.**
*Эта команда нужна для вывода на экран истории всех коммитов*

* git diff

*А вот эта нужна для просмотра разницы между текущим и закоммиченным файлом*
*Сравнение — это функция, анализирующая два входных набора данных и отображающая различия между ними. git diff представляет собой многоцелевую команду Git, которая инициирует функцию сравнения источников данных Git — коммитов, веток, файлов и т. д.*

* .gitingrone 

*Git рассматривает каждый файл в вашей рабочей копии как файл одного из трех нижеуказанных типов. прим. ![conflict-1.png](conflict-1.png) ![conflict-2.png](conflict-2.png)*

1. Отслеживаемый файл — файл, который был предварительно проиндексирован или зафиксирован в коммите.
2. Неотслеживаемый файл — файл, который не был проиндексирован или зафиксирован в коммите.
3. Игнорируемый файл — файл, явным образом помеченный для Git как файл, который необходимо игнорировать.

* Pull request 

**Pull requests can be used in conjunction with the Feature Branch Workflow, the Gitflow Workflow, or the Forking Workflow. But a pull request requires either two distinct branches or two distinct repositories, so they will not work with the Centralized Workflow. Using pull requests with each of these workflows is slightly different, but the general process is as follows:**

**A developer creates the feature in a dedicated branch in their local repo.**

1. The developer pushes the branch to a public Bitbucket repository.

2. The developer files a pull request via Bitbucket.

3. The rest of the team reviews the code, discusses it, and alters it.

4. The project maintainer merges the feature into the official repository and closes the pull request.

5. The rest of this section describes how pull requests can be leveraged against different collaboration workflows.