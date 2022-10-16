VKBot
========

Чат-бот на Java для ВКонтакте.
Идеально подходит как "Ассистент" в конференциях.

**ВНИМАНИЕ:**
Для работы бота необходима Java 8

ТЫ ПИДОР

## Начальная настройка:
1. Скачать и распаковать бота в рабочую среду вашей IDE
2. Изменить access_token, префиксы и другие значения
3. По необходимости добавить или изменить функционал
4. Скомпилировать и запустить как и любое Java приложение

## Смена префиксов:
* По умолчанию бот отзывается на пять префиксов: `!`, `фб`, `файнбот`, `вб`, `вкбот`
* Сменить их можно в главном классе бота

## Функционал:
* Список команд (Список всех команд бота `! команды`)
* Приветствие (Плагин преветствия, массив сообщений с ответами указан в модуле Messages)
* Случайные сиськи (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Posts)
* Случайные мемы (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Posts)
* Случайные мемы с 2ch (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Posts)
* Случайные девушки (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Postsy)
* Курс валют (Отображение основных курсов валют с сайта fixer.io, находится в модуле Sites)
* Шар восьмерка (Решает за вас, находится в модуле Messages)
* Дата и время (Показывает текущую дату и время, находится в модуле Messages)
* Онлайн серверов FineMine (Чтобы на сайт не заходить. Находится в модуле Sites)
* Случайное с FineMine (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Posts)
* Случайные школьницы (Берутся из паблика, указанного в передаваемых параметрах VK.getPosts(-groupID, postsLimit) внутри модуля Postsy)
* Отправка смайла (Отправляется смайл "Луна", находится в модуле Messages)
* Поиск видео по ВКонтакте (Поиск по фразе и отправка видео запросившему. Находится в модуле Messages)
* Поиск гифок по ВКонтакте (Поиск по фразе или смайлу и отправка гифки запросившему. Находится в Messages)
* Чат с ботом (Общение через iii.ru)
* Сокращение любых ссылок (Через VK)
* Музыка (Список музыки из ваших рекомендаций в ВК. Пока не работает)
* Отправка анонимных сообщений от имени бота (Находится в модуле Messages)
* Отправка случайных шуток с bash.im (Находится в модуле Sites)

## Примечание:
* Для того, чтобы узнать ID пользователя или паблика, используйте https://vk.com/linkapp
* Для того, чтобы узнать access_token, создайте приложение на странице https://vk.com/apps?act=manage и используйте эту ссылки, изменив айди приложения (Либо можете использовать мое) https://oauth.vk.com/authorize?client_id=60474390&scope=offline,notify,friends,photos,audio,video,pages,status,notes,messages,wall,docs,groups,notifications,stats,email&display=page&response_type=token&redirect_uri=https://oauth.vk.com/blank.html

* Если полсле запуска бота, авторизации в ВК не происходит, включите отладку и скопируйте ссылку из текста ошибки, открыв ссылку на подтверджение валидации через текстовый браузер links в Debian и пройдите проверку.

## Создание модулей:
* В папке modules находятся классы отвечающие за функционал, добавить новые или изменить существующие можно по их примеру
* Инициализация модулей происходит в главном классе мода

* Модули могут работать со всеми методами API вконтакте, новые методы можно добавить в классе VK внутри пакета api.

## Лицензия:
Код распространяется под лицензией [GPL V2](https://ru.wikipedia.org/wiki/GNU_General_Public_License) (General_Public_License V2)
