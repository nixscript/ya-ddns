# ya-ddns
DDNS Yandex

[![Build Status](https://travis-ci.org/nixscript/ya-ddns.svg?branch=master)](https://travis-ci.org/nixscript/ya-ddns)
[![GitHub License](https://img.shields.io/github/license/nixscript/ya-ddns.svg)](https://github.com/nixscript/ya-ddns/blob/master/LICENSE.md)
[![GitHub Release](https://img.shields.io/github/release/nixscript/ya-ddns.svg)](https://github.com/nixscript/ya-ddns/releases)

# Что нужно?
- ОС — Linux
- Установлен curl
- IP — белый, хоть и динамический (узнать у провайдера)
- Маршрутизатор настроен на проброс нужного порта до компьютера. В ADSL-модемах это названо «Виртуальный сервер». В маршрутизаторах может быть названо «Проброс» или «Перенаправление». По модели маршрутизатора/модема яндекс/гугл найдёт информацию, как это настроить.
- У вас есть доменное имя делегированное на DNS яндекса.

# Как пользоваться?
- Сохраните файл ya-ddns в любой удобной директории, желательно чтобы путь был латиницей.
- Внимательно прочитайте инструкции в комментариях, внутри скрипта, и действуйте согласно им.
- Добавьте запуск скрипта в Cron, через каждые 14400 секунд, или укажите свой интервал в скрипте и в Cron.
