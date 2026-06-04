
---
# Содержание
- [Cодержание](#содержание)
- [Задание](#задание)
	- [Your Architectural Kata is... Ding, Dong!](#your-architectural-kata-is-ding-dong)
	- [Ваша архитектурная ката это... Ding, Dong!](#ваша-архитектурная-ката-это-ding-dong!)
---
# Задание

## Your Architectural Kata is... Ding, Dong!

(Originally intended for embedded systems architects)

The DingDong is a wifi connected door bell and camera. It enables people to be notified if someone is at their door on their phone even before someone has pressed the button. If they have a delivery and are not at home they can tell the delivery guy to just leave it at the door. It also adds security as you have a record of anyone snooping around your house 24/7. You’re going to have figure out the device software and the web services that link everything back to the phone app.

Prioritised backlog: Play a loud ring; Run a WIFI host to receive a phone app connection that will send new wifi connection details and a password for changing those details; Send a notification to the web service when the button is pushed; Start a two way audio stream once the ring is acknowledged from a client; Start a video stream once the ring is acknowledged from a client; On button press switching from wifi client to wifi host to receive new connection details; Allow changing the password over an established wifi connection; Streaming video to a service to detect movement; Notifying a client of detected movement; Starting video and audio stream when detected movement is acknowledged from a client; Recording video and audio of a detected movement; Allowing a client to trigger a loud alarm

The hardware level controls are:

* Wifi that can host an unsecure connection or connect to secure wifi host.

* Video that can be streamed to a web service

* Audio that can be two-way streamed to a web service

* A button press interrupt

* Some pre-defined ring sounds stored in rom

* A small button that needs a needle to press

---

## Ваша архитектурная ката это... Ding, Dong!

(Изначально предназначено для архитекторов embedded-систем.)

**DingDong** — это дверной звонок с камерой, подключённый к Wi-Fi. Он позволяет людям получать уведомления на телефон, если кто-то находится у двери, даже до того, как человек нажал на кнопку звонка. Если пришла доставка, а хозяина нет дома, он может сказать курьеру оставить посылку у двери. Также устройство повышает безопасность, так как позволяет круглосуточно хранить запись всех, кто ходит рядом с домом.

Вам нужно спроектировать программное обеспечение устройства и веб-сервисы, которые связывают устройство с мобильным приложением.

Приоритизированный backlog:
1. Воспроизвести громкий звонок.
2. Запустить Wi-Fi host, чтобы принять подключение мобильного приложения, которое передаст новые данные для подключения к Wi-Fi и пароль для их изменения.
3. Отправить уведомление в веб-сервис при нажатии на кнопку.
4. Запустить двусторонний аудиопоток после подтверждения звонка клиентом.
5. Запустить видеопоток после подтверждения звонка клиентом.
6. При нажатии на кнопку переключаться из режима Wi-Fi client в режим Wi-Fi host, чтобы принять новые данные подключения.
7. Разрешить изменение пароля через уже установленное Wi-Fi-соединение.
8. Стримить видео в сервис для обнаружения движения.
9. Уведомлять клиента об обнаруженном движении.
10. Запускать видео- и аудиопоток, когда клиент подтвердил обнаруженное движение.
11. Записывать видео и аудио при обнаружении движения.
12. Разрешить клиенту запускать громкую тревогу.

## Низкоуровневые возможности устройства

- Wi-Fi, который может либо поднимать незащищённое соединение как host, либо подключаться к защищённой Wi-Fi-сети как client.
- Видео, которое можно стримить в веб-сервис.
- Аудио, которое можно передавать в обе стороны через веб-сервис.
- Прерывание по нажатию кнопки.
- Несколько заранее заданных звуков звонка, сохранённых в ROM.
- Маленькая кнопка, которую можно нажать только иглой.