---
lang: ru-RU
title: "Отчёт по лабораторной работе 6"
subtitle: "Адресация IPv4 и IPv6. Двойной стек"
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

Изучение принципов распределения и настройки адресного пространства на устройствах сети.

# Выполнение лабораторной работы

## Топология лабораторного стенда в GNS3

![Топология лабораторного стенда в GNS3](image/1.png){ #fig:001 width=80% }

## Настройка IPv4-адресации на PC1-akabrikosov

![Настройка IPv4-адресации на PC1-akabrikosov](image/2.png){ #fig:002 width=80% }

## Настройка IPv4-адресации на PC2-akabrikosov

![Настройка IPv4-адресации на PC2-akabrikosov](image/3.png){ #fig:003 width=80% }

## Настройка IPv4-адресации на Server-akabrikosov

![Настройка IPv4-адресации на Server-akabrikosov](image/4.png){ #fig:004 width=80% }

## Настройка интерфейсов маршрутизатора msk-akabrikosov-gw-01

![Настройка интерфейсов маршрутизатора msk-akabrikosov-gw-01](image/5.png){ #fig:005 width=80% }

## Проверка состояния интерфейсов маршрутизатора

![Проверка состояния интерфейсов маршрутизатора](image/6.png){ #fig:006 width=80% }

## Проверка связности с PC1-akabrikosov

![Проверка связности с PC1-akabrikosov](image/7.png){ #fig:007 width=80% }

## Проверка связности с PC2-akabrikosov

![Проверка связности с PC2-akabrikosov](image/8.png){ #fig:008 width=80% }

## Настройка IPv6-адресации на PC3-akabrikosov

![Настройка IPv6-адресации на PC3-akabrikosov](image/9.png){ #fig:009 width=80% }

## Настройка IPv6-адресации на PC4-akabrikosov

![Настройка IPv6-адресации на PC4-akabrikosov](image/10.png){ #fig:010 width=80% }

## Проверка IPv4- и IPv6-адресации на Server-akabrikosov

![Проверка IPv4- и IPv6-адресации на Server-akabrikosov](image/11.png){ #fig:011 width=80% }

## Настройка IPv6-интерфейсов маршрутизатора VyOS

![Настройка IPv6-интерфейсов маршрутизатора VyOS](image/12.png){ #fig:012 width=80% }

## Проверка интерфейсов маршрутизатора VyOS

![Проверка интерфейсов маршрутизатора VyOS](image/13.png){ #fig:013 width=80% }

## Проверка IPv6-связности с PC3-akabrikosov

![Проверка IPv6-связности с PC3-akabrikosov](image/14.png){ #fig:014 width=80% }

## Проверка IPv6-связности с PC4-akabrikosov

![Проверка IPv6-связности с PC4-akabrikosov](image/15.png){ #fig:015 width=80% }

## Проверка изоляции IPv4 и IPv6 подсетей

![Проверка изоляции IPv4 и IPv6 подсетей](image/16.png){ #fig:016 width=80% }

## Захват ARP-трафика на интерфейсе сервера

![Захват ARP-трафика на интерфейсе сервера](image/17.png){ #fig:017 width=80% }

## Захват ICMP-трафика IPv4

![Захват ICMP-трафика IPv4](image/18.png){ #fig:018 width=80% }

## Захват ICMPv6-трафика

![Захват ICMPv6-трафика](image/19.png){ #fig:019 width=80% }

## Топология сети с двумя локальными подсетями

![Топология сети с двумя локальными подсетями](image/20.png){ #fig:020 width=80% }

## Проверка IPv4 и IPv6 адресации на PC1-akabrikosov

![Проверка IPv4 и IPv6 адресации на PC1-akabrikosov](image/21.png){ #fig:021 width=80% }

## Проверка IPv4 и IPv6 адресации на PC2-akabrikosov

![Проверка IPv4 и IPv6 адресации на PC2-akabrikosov](image/22.png){ #fig:022 width=80% }

## Проверка настроенной адресации интерфейсов VyOS

![Проверка настроенной адресации интерфейсов VyOS](image/23.png){ #fig:023 width=80% }

## Проверка связности ping и trace между PC1 и PC2

![Проверка связности ping и trace между PC1 и PC2](image/24.png){ #fig:024 width=80% }


# Выводы по проделанной работе

## Вывод

В ходе работы:
- выполнено разбиение IPv4 и IPv6 адресных пространств на подсети;
- настроен двойной стек IPv4/IPv6 в GNS3;
- подтверждена связность внутри соответствующих подсетей;
- подтверждена изоляция IPv4 и IPv6 сегментов (кроме Dual Stack сервера);
- выполнен анализ ARP, ICMP, ICMPv6 в захваченном трафике.
