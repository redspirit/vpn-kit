# VPN-KIT

## Что это?
Тут представлен небольшой конфиг в виде Docker Compose файла для запуска нескольких VPN-серверов, а именно:
- VLESS с XTLS-Reality (панель 3X-UI)
- Wireguard (панель WG-Easy)
- IPSec (потому что имеет встроенную поддержку на многих Wi-Fi роутерах, даже старых)

## Установка
После клонирования репозиторий добавьте в корень файлы:

`ipsec.env`:

```env
VPN_USER=ipsec
VPN_PASSWORD=[PASSWORD]
VPN_IPSEC_PSK=[KEY]
```

`wg.env`:

```env
WG_HOST=[HOST_OR_IP]
PASSWORD_HASH=[PASS_HASH] 
```
Подробнее о настройке: https://github.com/wg-easy/wg-easy

Далее запуск

```shell
docker compose up -d
```
