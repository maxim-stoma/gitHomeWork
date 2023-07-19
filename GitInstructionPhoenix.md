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

## 