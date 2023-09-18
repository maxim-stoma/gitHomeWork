# Инструкция по работе с удаленными репозиториями

## Копирование удаленнго репозитория в локальную папку
1. Создаем копию удаленного репозитория (**fork**) в свой аккаунт на GitHUB\
для копирования заходим в интересующий на репоситорий и нажимаем кнопку **FORK""\
!["RepositForCopy"](RepositForCopy.png)
в появившемся окне нажимаем кнопку **CREATE FORK**\
!["ForkReposit"](ForkReposit.png)
в итоге получаем\
![forkResult](ForkResult.png)
копируем ссылку на удаленный репоситорий и переходим в VisualStudioCode
![copyRefDeposit](CopyRefDeposit.png)
2. Создание локальной копии удаленного репозитория (**clone**)
Создаем пустую папку на копьютере и открываем ее в VSCode\
Проверяем что в ней отсутствуют какие-либо репозитории коммандой **git status**\
![Alt text](EmptyDir.png)
Создаем копию удаленного репоситория в локальной папке\
**git clone <Сcылка cкопированная с GitHUB>**
![CloneReposit](CloneReposit.png)
Переходим в директорию со скопированным репозиторием
cd <имя директории>
![ChangeDir](ChangeDir.png)

## Создаем новую ветку и переходим в нее
 * **git branch** - просмотр существующих веток
 * **git branch <branch_name>** - создание ветки с именем *branch_name*
 * **git checkout <branch_name>** - переход в ветку с именем *branch_name*
![BranchMade](BranchMade.png)