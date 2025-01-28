# VPN-KIT

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
