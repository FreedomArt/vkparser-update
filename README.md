# Парсинг контента ВКонтакте

PHP парсер, который позволяет брать разные посты из групп ВК и добавлять в свою группу.
Обновленный всё согласно https://vk.com/dev/versions и https://vk.com/dev.php?method=constant_version_updates

## Перед началом работы
Прежде всего проверьте, включен ли SQLite3 (http://php.net/manual/ru/sqlite3.installation.php) и cURL (https://stackoverflow.com/questions/1347146/how-to-enable-curl-in-php-xampp). Настройка может отличаться в зависимости от ОС, условий запуска (хостинг) и т.д.

## Настройка
Для начала работы необходимо открыть example.config.php и сделать следующее:

1. Указать `VK_GROUP_ID` - ID своей группы;
2. Получить `VK_ACCESS_TOKEN`. В настройках (`example.config.php`) описана инструкция, как это сделать. Приложения создаются по ссылке [здесь](https://vk.com/apps?act=manage);
3. Перечислите группы, из которых будет забираться контент в массиве `$groups`;
4. Переименовать `example.config.php` в `config.php`;
5. Запустите скрипт через браузер или CRON (есть также опция - разрешать запуск не через CRON, или нет). Пример команды для CRON указан в том же файле настроек.

Готово. Теперь посты из других групп будут добавляться в вашу. В файле настроек (`config.php`) есть ещё много различных опций с описанием их работы.
Вы можете изменить их под ваши нужды.

DONATE:
