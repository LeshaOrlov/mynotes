# Docker
Created вторник 16 Февраль 2021

Список образов
	
	docker images


Список запущенных контейнеров
	
	docker ps


Запуск контейнера
	
	docker run myNameImage


Запуск контейнера в фоне
	
	docker run -d myNameImage


Создание контейнера
	
	docker build -t myNameImage


Запуск контейнера c пробросом порта
	
	docker run -p 80:80 myNameImage


Удалить контейнер
	
	docker rm <CONTAINERID>


Удалить все контейнеры
	
	docker rm $(docker ps --qa)


Остановить контейнер

	docker stop my_container

Сборка
------
На основе Dockerfile  в текущей директории
	
	docker build --tag my-image


Диски
-----

