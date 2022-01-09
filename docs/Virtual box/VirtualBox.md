# VirtualBox
Created четверг 18 Февраль 2021

Auto-resize screen
------------------
Чтобы работало авто-разрешение экрана вы должны использовать графический контроллер VBoxVGA 
Откройте настройки 
Machine Settings - Display - Graphics Controller
Установите VBoxSVGA
Устоновите virtualbox guest utils с установочного диска или команды
	sudo apt-get install virtualbox-guest-additions-iso
	

Включить аппаратное ускорение Intel
-----------------------------------
Перейти в папку  с программой
	cd "C:\Program Files\Oracle\VirtualBox"

Посмотреть список виртуальных машин
	VBoxManage.exe list vms

Выполнить команду
	VBoxManage.exe modifyvm "Ubuntu 20.04" --nested-hw-virt on
	

