# ya-ddns
DDNS Yandex

[![Build Status](https://travis-ci.org/nixscript/ya-ddns.svg?branch=master)](https://travis-ci.org/nixscript/ya-ddns)
[![GitHub License](https://img.shields.io/github/license/nixscript/ya-ddns.svg)](https://github.com/nixscript/ya-ddns/blob/master/LICENSE.md)
[![GitHub Release](https://img.shields.io/github/release/nixscript/ya-ddns.svg)](https://github.com/nixscript/ya-ddns/releases)

Если вы пользуетесь сервисом Яндекса «Почта для домена», вы легко можете организовать бесплатный DDNS.
Этот скрипт написано по этой статье, где скрипт написан на Python: https://habrahabr.ru/sandbox/102896/

# Что такое DDNS?
Это связывание доменного имени с IP-адресом компьютера в сети или интернете, не зависимо от того, меняется IP при каждом подключении или нет. В итоге набирая в адресной строке yndex.ru мы попадаем именно на сервер Яндекса, а не куда-то ещё.

# Для чего нам DDNS?
Допустим вы хотите подключиться к своему домашнему компьютеру удалённо. Обычно провайдер не выделяет статических IP-адресов частным клиентам, а динамический IP меняется при каждом переподключении к интернету, что значительно осложняет подключение из вне к домашнему компьютеру. С помощью DDNS можно избежать этой проблемы, и организовать дома даже собственный веб-сервер, с простым доступом.

# Что нужно?
- ОС — Linux
- Установлен curl
- IP — белый, хоть и динамический (узнать у провайдера).
- Маршрутизатор настроен на проброс нужного порта до компьютера. В ADSL-модемах это названо «Виртуальный сервер». В маршрутизаторах может быть названо «Проброс» или «Перенаправление». По модели маршрутизатора/модема яндекс/гугл найдёт информацию, как это настроить.
- У вас есть доменное имя делегированное на DNS яндекса. Об этом подробно узнаете у продавцов доменных имён.

# Как пользоваться?
- Сохраните файл ya-ddns в любой удобной директории, желательно чтобы путь был латиницей.
- Внимательно прочитайте инструкции в комментариях, внутри скрипта, и действуйте согласно им.
- Добавьте запуск скрипта в Cron, через каждые 14400 секунд, или укажите свой интервал в скрипте и в Cron.

Подробности по API Яндекса здесь: https://tech.yandex.ru/pdd/doc/about-docpage/
Если возникнут проблемы или ошибки, API Яндекса поможет разобраться.
