# Система рассписаний для коллежда связи

## Запуск
 
### !Необходимо проверить настройки подключения к локальному серверу PostgeSQL бд в файле appsetings.json 
**Hakaton.API** - миграция для базы данных нужно выполнить командной "dotnet ef database update". Сервис запускается командой "dotnet run", либо с помощью Visual Studio 2022

**schedule_scc** - react приложение, запускается командной "npm i" "npm run dev"
**scheduleAPK** - мобильное приложение на kotlin, для запуска необходимо открыть проект с помощью Android Studio и наверху где указывается ветка разработки, выбрать Group.Для того чтобы работало с БД надо использовать команду "ngrok http 5057" через консоли в папке самого проекта. Скопировать строку перед -> http://localhost:5057. После этого, открыть файл по пути "ScheduleAPK\app\src\main\java\com\example\schedule\ApiClient" Изменить строку "BASE_URL" на скопированную строку. После чего подключить телефон через кабель зарядки / через wi-fi !(Необходимо в настройках разработчика включить режим отладки).
После запустить проект с помощью Android Studio 