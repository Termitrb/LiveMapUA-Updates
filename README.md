# LiveMapUA Updates

OTA-репозиторій для оновлень LiveMapUA.

## Постійна адреса OTA

https://raw.githubusercontent.com/Termitrb/LiveMapUA-Updates/main/update.json

## Схема оновлення

1. Збирається новий APK тим самим ключем підпису.
2. Збільшується `versionCode`.
3. APK додається до GitHub Release.
4. Для APK рахується SHA-256.
5. Оновлюється `update.json`.
6. LiveMapUA завантажує APK та перевіряє:
   - SHA-256
   - packageName
   - versionCode
   - Android перевіряє підпис APK

## Безпека

Не зберігати в цьому репозиторії:

- keystore
- паролі
- Telegram API hash
- токени
- приватні ключі
