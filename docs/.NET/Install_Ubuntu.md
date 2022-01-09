# Install Ubuntu
Created четверг 18 Февраль 2021

Ubuntu 20.04
 
Добавить ключ подписывания пакета Майкрософт в список доверенных ключей и добавить репозиторий пакетов.
	wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
	sudo dpkg -i packages-microsoft-prod.deb

Установите один из следующих пакетов:

Установка пакета SDK
	sudo apt-get update; \
	  sudo apt-get install -y apt-transport-https && \
	  sudo apt-get update && \
	  sudo apt-get install -y dotnet-sdk-5.0


Установка среды выполнения без SDK
	sudo apt-get update; \
	  sudo apt-get install -y apt-transport-https && \
	  sudo apt-get update && \
	  sudo apt-get install -y aspnetcore-runtime-5.0


Установка среды выполнения dotnet без поддержки ASP.NET
	sudo apt-get install -y dotnet-runtime-5.0


Подробнее: <https://docs.microsoft.com/ru-ru/dotnet/core/install/linux-ubuntu>

