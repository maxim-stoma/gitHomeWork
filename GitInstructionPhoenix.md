# Инструкция по работе с удалёнными репозиториями

## Создание копии (удаленного) репозитория

Для начала работы с центральным репозиторием, следует создать копию оригинального проекта со всей его историей локально.

Клонируем репозиторий, используя протокол http:

* *git clone http://user@somehost:port/~user/repository/project.git*

Клонируем репозиторий с той же машины в директорию myrepo:

* *git clone /home/username/project myrepo*

Клонируем репозиторий, используя безопасный протокол ssh:

* *git clone ssh://user@somehost:port/~user/repository*

У git имеется и собственный протокол:

* *git clone git://user@somehost:port/~user/repository/project.git/*

Импортируем svn репозиторий, используя протокол http:

* *git svn clone -s http://repo/location*

-s – понимать стандартные папки SVN (trunk, branches, tags)

## Забираем изменения из центрального репозитория

Для синхронизации текущей ветки с репозиторием используются команды git fetch и git pull.

git fetch — забрать изменения удаленной ветки из репозитория по умолчания, основной ветки; той, которая была использована при клонировании репозитория. Изменения обновят удаленную ветку (remote tracking branch), после чего надо будет провести слияние с локальной ветку командой git merge.

* *git fetch /home/username/project* — забрать изменения из определенного репозитория.

Возможно также использовать синонимы для адресов, создаваемые командой git remote:

* *git remote add username-project /home/username/project*

* *git fetch username-project* — забрать изменения по адресу, определяемому синонимом.

Естественно, что после оценки изменений, например, командой git diff, надо создать коммит слияния с основной:

* *git merge username-project/master*

Команда git pull сразу забирает изменения и проводит слияние с активной веткой.

* *git pull username-project --tags*

Как правило, используется сразу команда git pull.

## Вносим изменения в удаленный репозиторий

После проведения работы в экспериментальной ветке, слияния с основной, необходимо обновить удаленный репозиторий (удаленную ветку). Для этого используется команда git push.

Отправить свои изменения в удаленную ветку, созданную при клонировании по умолчанию:

* *git push*

Отправить изменения из ветки master в ветку experimental удаленного репозитория:

* *git push ssh://yourserver.com/~you/proj.git master:experimental*

В удаленном репозитории origin удалить ветку experimental:

* *git push origin :experimental*

В удаленную ветку master репозитория origin (синоним репозитория по умолчанию) ветки локальной ветки master:

* *git push origin master:master*

Отправить метки в удаленную ветку master репозитория origin:

* *git push origin master --tags*

Изменить указатель для удаленной ветки master репозитория origin (master будет такой же как и develop)

* *git push origin origin/develop:master*

Добавить ветку test в удаленный репозиторий origin, указывающую на коммит ветки develop:

* *git push origin origin/develop:refs/heads/test* 