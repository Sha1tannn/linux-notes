# Journalctl 

## Возможности journalctl 

- journalctl -u nginx -f - проверка логов nginx в реальном времени
- journalctl -u nginx - проверка логов сервиса nginx
- journalctl -u nginx -n 20 - показать последние 20 записей nginx
- journalctl -b (boot) - показывает логи текущей сессии
- journalctl --list-boots - список сессий
- journalctl --since today ( --since "1 hour/10minutes ago) - првоерка логов за определенное время 
- journactl - p err/warning/alert/crit/emerg и т.д (priority) - показывает опредленные записи 
- journactl -k - посмотреть логи ядра