<br>
<p align="center">
<img src="files/static/logoPodman.png" width="200" height ="200" />
<br><br>

# Podman - Быстый старт
Присоединяйтесь к нам - [Youtube](https://www.youtube.com/channel/UCqC3c7UHtwoX2wy7fdHc6gg) и [Telegram](https://t.me/devops_mops)

## Содержание
- [Что такое Podman?](#Что-такое-Podman?)
- [Установка Podman](#Установка-Podman)
- [Базовые команды](#Базовые-команды)

## Что такое Podman?
Podman - это консольная утилита для запуска OCI containers and pods (поэтому он PODman :) )
<br>
Можно рассматривать Podman как Daemonless Docker.

## Установка Podman
Podman так же как Docker поддерживает установку на разных ОС (Windows, Linux, macOS)
https://podman.io/getting-started/installation

## Базовые команды

Команды Podman основаны на командах Docker. На оффициальном сайте даже предлагаю сделать алиас:
```
alias docker=podman
```

Не уверен, что это хорошая идея, так как оба слова одинаковой длинны :)
<br>

И если делать алиас, то сокращать так сокращать
```
alias p=podman
```
<br>

Посмотреть версию
```
podman version
```
<br>

Вывести подробную информацию о конфигурации
```
podman info
```
<br>

Загрузить образ в репозиторий
```
podman pull
```
<br>

Загрузить образ из репозитория
```
podman push
```
<br>

Загрузить список запущенный контейнеров
```
podman ps
```
<br>

Вывести список контейнеров, запущенных другими Container runtime
```
podman ps --sync --external --all
```
<br>

Запустить контейнер
```
podman run -d busybox sleep 3600
```
<br>

Остановить контейнер
```
podman stop --latest
```
<br>

Вывести список загруженных образов
```
podman images
```
<br>