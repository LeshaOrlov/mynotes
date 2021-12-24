# install
Created четверг 23 Декабрь 2021

dism.exe /online /enable-feature /featurename:microsoft-windows-subsystem-linux /all /norestart

dism.exe /online /enable-feature /featurename:virtualmachineplatform /all /norestart

wsl --set-default-version 2

wsl --update

restart windows

