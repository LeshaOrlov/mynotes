# vscode sftp
Created пятница 12 Февраль 2021

установим расширение **sftp**
выберем папку для работы
редактируем файл **sftp.json**
	{
		"name": "Ubuntu server",
		"host": "192.168.1.102",
		"protocol": "sftp",
		"port": 22,
		"username": "alex",
		"password": "123",
		"remotePath": "/home/alex/sourcecode/node_test",
		"uploadOnSave": true,
		"downloadOnOpen": true
	}

Изменим настройку VSCode
*VScode > File > Preferences > Settings*
Select "downloadWhenOpenInRemoteExplorer" then restart vscode.

