# ChatUygulamasi

Python ile yazılmış, soket tabanlı çok kullanıcılı sohbet uygulaması.

- `server.py` – TCP sunucusu; her istemciyi ayrı bir thread'de dinler ve gelen mesajı diğer istemcilere iletir
- `client.py` – Tkinter arayüzlü istemci; isimle katılma, mesaj gönderme ve çevrimiçi kullanıcı listesi

## Teknolojiler

Python 3, `socket`, `threading`, `tkinter` (yalnızca standart kütüphane, ek paket gerekmez)

## Çalıştırma

```bash
cd "visual studio code"
python server.py
```

Ardından her kullanıcı için ayrı bir terminalde:

```bash
python client.py
```

Not: Sunucu varsayılan olarak yalnızca bu bilgisayardan (`127.0.0.1:10319`) bağlantı kabul eder. Bağlantılar şifrelenmediği ve kimlik doğrulaması olmadığı için uygulama eğitim amaçlıdır; internete açık bir ağda çalıştırılmamalıdır.
