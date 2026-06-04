# Systemd

## Что такое systemd?

systemd - это система инициализации и управления сервисами в Limux.

Она запускает процессы после загрузки системы, следит за службами и позволяет управлять ими.

## Что такое service?

Service (Служба) - это фоновоый процесс, который работает без прямого участия пользователя.

## Команды systemd

- systemctl status ssh - статус службы
- systemctl start ssh - запуск службы
- systemctl stop ssh - остановка службы
- systemctl restart nginx - перезапуск службы
- systemctl reload ssh - перечитывает конфигурацию службы без полного перезапуска
- systemctl enable ssh - добавление службы в автозагрузку
- systemctl disalbe ssh - убрать из автозагрузки
- systemctl is-enabled ssh - проверка автозагрузки
- systemctl list-untits --type=service (--state=running) - проверка всех служб, активных и нет
- systemctl mask/unmask ssh - сервис нельзя будет запустить

## Статусы служб

active (running) — сервис запущен и работает
inactive (dead) — сервис остановлен
failed — сервис упал с ошибкой
activating — сервис запускается
deactivating — сервис останавливается

