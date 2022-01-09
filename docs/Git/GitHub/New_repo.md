# New repo
Created среда 02 Июнь 2021

Предположим, что у вас уже есть какой-то проект, для которого вы хотите создать Git репозиторий. Создание репозитория выполняется точно также, как описано выше. Перейдите в папку проекта:
	cd myproject

Создайте репозиторий:
	git init

Теперь можно добавить все файлы в индекс и сделать первый коммит:
	git add -A
	git commit -m "First commit."

Как создать удаленный репозиторий (на примере Github)

Вы создали локальный репозиторий, теперь, например, вам нужно добавить его на Github, тем самым вы фактически создадите удаленный репозиторий.

Перейдите на <https://githib.com> и войдите в свой аккаунт. Нажмите кнопку New repository (Новый репозиторий). На открывшейся странице введите имя репозитория (Repository name) и нажмите кнопку Create repository.

В своем локальном репозитории теперь выполните команду:

	git remote add origin https://github.com/username/myproject.git


Данная команда добавит удаленный репозиторий с именем origin, который указывает на ваш Github-репозиторий. Пока мы только добавили запись об удаленном репозитории.

Теперь можно выполнить команду git push, чтобы отправить все ваши изменения на удаленный репозиторий:
	git push -u origin master

Вам нужно будет ввести логин и пароль аккаунта в Github. Результат команды будет примерно следующим:
	git init
	$ git push -u origin master
	Username for 'https://github.com': youremail@email.com
	Password for 'https://youremail@email.com@github.com':
	Counting objects: 4, done.
	Delta compression using up to 4 threads.
	Compressing objects: 100% (2/2), done.
	Writing objects: 100% (4/4), 252 bytes | 252.00 KiB/s, done.
	Total 4 (delta 0), reused 0 (delta 0)
	remote:
	remote: Create a pull request for 'master' on GitHub by visiting:
	remote: https://github.com/username/myproject/pull/new/master
	remote:
	To https://github.com/username/myproject.git
	* [new branch] master -> master
	Branch 'master' set up to track remote branch 'master' from 'origin'.
	


В команде git push мы использовали ключ -u. Данный ключ используется для того, чтобы связать локальную ветку master с удаленной origin/master (в нашем случае удаленной ветки не существовало, она автоматически была создана). Так как связь установлена, то последующие выполнения git push из ветки мастер можно выполнять без указания веток. То есть вместо git push origin master), можно просто выполнять команду git push.

