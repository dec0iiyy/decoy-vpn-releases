# Decoy VPN

VPN-клиент для Android на движке [xray-rust](https://github.com/aimalygin/xray-rust). Добавь свою подписку или ключ и подключайся в одно касание.

Поддерживаются VLESS (Reality, XTLS Vision), VMess, Trojan, Shadowsocks, Hysteria 2, SOCKS5 и HTTP. Подписки в формате base64-списка ссылок, раздельное туннелирование по приложениям, плитка в быстрых настройках.

## Установка

1. Открой [последний релиз](https://github.com/dec0iiyy/decoy-vpn-releases/releases/latest).
2. Скачай APK под свой телефон:
   - `arm64-v8a` — почти все современные телефоны;
   - `armeabi-v7a` — старые 32-битные;
   - `universal` — если не уверен, подойдёт везде, но весит больше.
3. Открой файл и разреши установку из этого источника.

Нужен Android 8.0 или новее.

## Проверка подлинности

Каждый релиз подписан одним и тем же ключом. Отпечаток сертификата (SHA-256):

```
B1:35:11:4D:AB:24:59:70:4C:24:F2:43:3B:2F:A0:6A:CB:D9:51:C7:E2:48:5E:AB:54:32:1D:46:E4:6B:D4:58
```

Проверить: `apksigner verify --print-certs DecoyVPN-*.apk`. Контрольные суммы файлов лежат в `SHA256SUMS.txt` в каждом релизе.

## Исходный код

Код приложения закрыт. Сторонние компоненты распространяются под своими лицензиями:

- **xray-rust** — [MPL-2.0](https://github.com/aimalygin/xray-rust/blob/main/LICENSE). Исходники: [upstream](https://github.com/aimalygin/xray-rust) и [форк с правками для Decoy](https://github.com/dec0iiyy/xray-rust).
- Compose Multiplatform, AndroidX, Kotlin, kotlinx, Ktor, Koin, Haze и другие библиотеки — Apache-2.0 или MIT.

## Обратная связь

Нашёл баг или есть идея — открой [issue](https://github.com/dec0iiyy/decoy-vpn-releases/issues).
