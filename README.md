# Corne RU

Конфигурация русской split-клавиатуры Corne на ZMK.

## Текущий стабильный кандидат

Первый этап стабилизации сохраняет:

- текущую раскладку и макросы;
- ZMK `v0.2`;
- платы `nice_nano`;
- тайм-ауты сна;
- передачу уровней заряда половин.

Из общего `config/corne.conf` удалены принудительные роли Bluetooth Central/Peripheral и экспериментальные BLE-параметры. Роли половин задаются shield-конфигурациями `corne_left` и `corne_right`.

## Сборка

После каждого push GitHub Actions собирает:

- `corne_left`;
- `corne_right`;
- `settings_reset`.

Перед прошивкой и перепривязкой прочитайте [инструкцию полного сброса](docs/02_RESET_FLASH_WINDOWS.md).

## Документация

- [Инженерный аудит](docs/01_ENGINEERING_AUDIT.md)
- [Сброс, прошивка и подключение Windows](docs/02_RESET_FLASH_WINDOWS.md)
