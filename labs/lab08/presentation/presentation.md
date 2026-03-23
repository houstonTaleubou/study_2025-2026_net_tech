---
lang: ru-RU
title: "Отчёт по лабораторной работе 8"
subtitle: "Адресация IPv4 и IPv6. Настройка маршрутизации"
author: "Талебу Тенке Франк Устон"
institute: "Российский университет дружбы народов, Москва, Россия"
theme: metropolis
aspectratio: 169
section-titles: true
toc: false
slide_level: 2
header-includes:
  - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
  - \usepackage{polyglossia}
  - \setmainlanguage{russian}
  - \setotherlanguage{english}
  - \setmainfont{DejaVu Serif}
  - \setsansfont{DejaVu Sans}
  - \setmonofont{DejaVu Sans Mono}
---

# Цели и задачи работы

## Цель лабораторной работы

Изучение принципов маршрутизации в IPv4- и IPv6-сетях и принципов настройки сетевого оборудования в среде GNS3.

# Выполнение лабораторной работы

## Топология в GNS3

![Топология сети в GNS3](image/1.png){ #fig:001 width=85% }

## Настройка IPv6 на PC1

![Настройка IPv6 на PC1](image/2.png){ #fig:002 width=85% }

## Настройка IPv6 на PC2

![Настройка IPv6 на PC2](image/3.png){ #fig:003 width=85% }

## Подготовка gw-01

![Подготовка gw-01](image/4.png){ #fig:004 width=85% }

## Адресация gw-01

![Настройка интерфейсов gw-01](image/5.png){ #fig:005 width=85% }

## Подготовка gw-02

![Подготовка gw-02](image/6.png){ #fig:006 width=85% }

## Адресация gw-02

![Настройка интерфейсов gw-02](image/7.png){ #fig:007 width=85% }

## Подготовка и адресация gw-03

![Подготовка gw-03](image/8.png){ #fig:008 width=85% }

## Подготовка и адресация gw-03

![Настройка интерфейсов gw-03](image/9.png){ #fig:009 width=85% }

## Проверка RA на оконечных устройствах

![Проверка IPv6 на PC1](image/10.png){ #fig:010 width=85% }

## Проверка RA на оконечных устройствах

![Проверка IPv6 на PC2](image/11.png){ #fig:011 width=85% }

## Ping с gw-01 до настройки маршрутизации

![Проверка связности с gw-01](image/12.png){ #fig:012 width=85% }

## Анализ трафика до RIP (gw-01 ↔ gw-03)

![Анализ трафика до RIP](image/13.png){ #fig:013 width=85% }

## Настройка RIP на gw-01

![RIP на gw-01](image/14.png){ #fig:014 width=85% }

## Настройка RIP на gw-02

![RIP на gw-02](image/15.png){ #fig:015 width=85% }

## Настройка RIP на gw-03

![RIP на gw-03](image/16.png){ #fig:016 width=85% }

## Проверка связности после включения RIP

![Проверка после RIP](image/17.png){ #fig:017 width=85% }

## Анализ трафика после RIP

![Трафик ICMP и RIP](image/18.png){ #fig:018 width=85% }

## Туннель SIT на gw-01

![Туннель SIT на gw-01](image/19.png){ #fig:019 width=85% }

## Туннель SIT на gw-02

![Туннель SIT на gw-02](image/20.png){ #fig:020 width=85% }

## Статическая маршрутизация IPv6

![Статический IPv6-маршрут на gw-01](image/21.png){ #fig:021 width=85% }

## Статическая маршрутизация IPv6

![Статический IPv6-маршрут на gw-02](image/22.png){ #fig:022 width=85% }

## Проверка с PC1: ping e trace до PC2

![PC1 → PC2: ping/trace](image/23.png){ #fig:023 width=85% }

## Проверка с PC2: ping e trace до PC1

![PC2 → PC1: ping/trace](image/24.png){ #fig:024 width=85% }

## Трафик IPv6 при передаче через IPv4

![Трафик при работе туннеля](image/25.png){ #fig:025 width=85% }

## Где видна информация о прохождении через туннель

![Инкапсуляция IPv6 em IPv4](image/26.png){ #fig:026 width=85% }

# Выводы по trabalho

## Вывод

В GNS3 настроена сеть с VyOS и VPCS, выполнена адресация IPv4/IPv6 и проведена проверка связности. Динамическая маршрутизация IPv4 (RIP) обеспечила доступность удалённых IPv4-сетей. Туннель SIT и статические маршруты IPv6 обеспечили обмен трафиком между удалёнными IPv6-сегментами. Анализ Wireshark подтвердил обмен ARP/ICMP/RIP и наличие инкапсуляции IPv6-пакетов внутри IPv4 при передаче через туннель.
