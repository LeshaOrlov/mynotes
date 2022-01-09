# dotnet command
Created воскресенье 14 Февраль 2021

dotnet
Пакет SDK для .NET Core (3.1.403)
Использование: dotnet [runtime-options] [path-to-application] [arguments]

Запуск приложения .NET Core.

runtime-options:
  --additionalprobingpath <path>   Путь к политике проверки и проверяемым сборкам.
  --additional-deps <path>         Путь к дополнительному файлу deps.json.
  --fx-version <version>           Версия установленной общей платформы, которую следует использовать для запуска приложения.
  --roll-forward <setting>         Накат до версии платформы (LatestPatch, Minor, LatestMinor, Major, LatestMajor, Disable).

path-to-application:
  Путь к DLL-файлу приложения, который необходимо выполнить.

Использование: dotnet [sdk-options] [command] [command-options] [arguments]

Выполнение команды пакета SDK для .NET Core.

sdk-options:
  -d|--diagnostics  Включение выходных данных диагностики.
  -h|--help         Показать справку командной строки.
  --info            Отображение сведений о .NET Core.
  --list-runtimes   Отображение установленных сред выполнения.
  --list-sdks       Отображение установленных пакетов SDK.
  --version         Отображение используемой версии пакета SDK для .NET Core.

Команды SDK:
  [add](./dotnet_command/dotnet_add.md)               Добавление пакета или ссылки в проект .NET.
  [build](./dotnet_command/dotnet_build.md)             Сборка проекта .NET.
  build-server      Взаимодействие с серверами, запущенными в ходе сборки.
  clean             Очистка выходных данных сборки проекта .NET.
  help              Показать справку командной строки.
  list              Вывод списка ссылок на проекты в проекте .NET.
  msbuild           Выполнение команд Microsoft Build Engine (MSBuild).
  [new](./dotnet_command/dotnet_new.md)               Создание нового файла или проекта .NET.
  nuget             Предоставление дополнительных команд NuGet.
  pack              Создание пакета NuGet.
  [publish](./dotnet_command/dotnet_publish.md)           Публикация проекта .NET для развертывания.
  remove            Удаление пакета или ссылки из проекта .NET.
  restore           Восстановление зависимостей, указанных в проекте .NET.
  run               Сборка и запуск проекта .NET.
  sln               Изменение файлов решения Visual Studio.
  store             Сохранение указанных сборок в хранилище пакетов среды выполнения.
  test              Запуск модульных тестов с помощью средства, указанного в проекте .NET.
  tool              Установка и настройка инструментов, расширяющих возможности .NET.
  vstest            Выполнение команд Microsoft Test Engine (VSTest).

Дополнительные команды из входящих в пакет инструментов:
  dev-certs         Создание сертификатов разработки и управление ими.
  fsi               Запуск F# Interactive / выполнение скриптов F#.
  sql-cache         Инструменты командной строки кэша SQL Server.
  user-secrets      Управление развертыванием секретов пользователей.
  watch             Запуск наблюдателя за файлами, который выполняет команду при изменении файлов.

Для получения дополнительных сведений о команде выполните команду "dotnet [команда] --help".

