## Тестовое задание 

[mock server](https://github.com/MrCelestis/mock-interview-api)
*в коде отсутствует обработка cors - необходимо установить пакет cors и указать app.use(cors()) в app.js*


1. Реализованы все пункты функционала приложения

- На старте приложение должно отправить запрос для загрузки данных о пакетах
- Каждый пакет должен быть представлен в виде карточки
	- Заголовок должен отображать имя пакета. В случае если имя составное (через /), первая часть должна быть выделена цветом
	- Тело должно содержать число скачек и зависимостей. В случае если число превышает 1000, оно должно быть округлено вниз до тысяч с буквой «К»; в случае если превышает 1000000, то до миллионов с буквой «М».
	- При наведении курсора на карточку её заголовок должен быть подсвечен, а также другим цветом должны быть подсвечены заголовки всех карточек пакетов, находящихся в зависимостях у выделенного пакета
- Список пакетов должен быть скроллируемым
- Пользователь должен иметь возможность фильтровать пакеты по названию
- Пользователь должен иметь возможность перезагрузить все данные по кнопке или иным способом

2. Написаны тесты к компоненту ```AppComponent ``` и сервису ```PackageService```
3. Добавлены автоматизированные инструменты проверки кода ```eslint``` и ```prettier```