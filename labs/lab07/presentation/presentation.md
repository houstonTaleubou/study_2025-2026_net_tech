---
lang: ru-RU
title: "Отчёт по лабораторной работе 7"
subtitle: "Адресация IPv4 и IPv6. Настройка DHCP"
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

# Цели и задачи

## Цель лабораторной работы

Получение навыков настройки службы DHCP на сетевом оборудовании для распределения адресов IPv4 и IPv6.

# Выполнение лабораторной работы

## Топология стенда (IPv4)

![Топология лабораторного стенда в GNS3](image/1.png){ width=80% }

## Базовая настройка VyOS

![Настройка IPv4-адреса интерфейса eth0](image/2.png){ width=80% }

## Настройка DHCP-сервера (IPv4)

![Настройка DHCP-сервера на VyOS](image/3.png){ width=80% }

## Получение адреса на клиенте (PC1)

![Получение IP-адреса по DHCP на PC1](image/4.png){ width=80% }

## Проверка связности (IPv4)

![Проверка IPv4-конфигурации и ping](image/5.png){ width=80% }

## Статистика и аренды DHCP (IPv4)

![Статистика DHCP-сервера](image/6.png){ width=80% }

## Журнал DHCP и этапы обмена

![Журнал работы DHCP-сервера](image/7.png){ width=80% }

## Анализ захваченного трафика (DHCP)

![Анализа DHCP](image/8.png){ width=80% }

# Настройка IPv6

## Расширение топологии (IPv6)

![Расширенная топология лабораторного стенда](image/9.png){ width=80% }

## Настройка IPv6-адресов на VyOS

![Настройка IPv6-адресов на интерфейсах VyOS](image/10.png){ width=80% }

## Настройка RA + DHCPv6 Stateless (eth1)

![Настройка Router Advertisements и DHCPv6 Stateless](image/11.png){ width=80% }

## Проверка конфигурации сервисов на VyOS

![Просмотр конфигурации DHCPv4 и DHCPv6](image/12.png){ width=80% }

## Проверка клиента PC2 (Stateless)

![Проверка IPv6-настроек на PC2](image/13.png){ width=80% }

## Проверка связности (IPv6)

![Ping IPv6-адреса маршрутизатора](image/14.png){ width=80% }

## Получение параметров по DHCPv6 (Stateless)

![Получение параметров по DHCPv6 Stateless](image/15.png){ width=80% }

## Аренды DHCPv6 в Stateless-режиме

![Состояние аренд DHCPv6](image/16.png){ width=80% }

## Анализ трафика (Stateless DHCPv6)

![Анализ DHCPv6-пакетов в анализаторе трафика](image/17.png){ width=80% }

## Настройка RA + DHCPv6 Stateful (eth2)

![Настройка DHCPv6 Stateful на VyOS](image/18.png){ width=80% }

## Начальные настройки клиента PC3 (до DHCPv6)

![Начальные IPv6-настройки на PC3](image/19.png){ width=80% }

## Получение IPv6 по DHCPv6 Stateful (PC3)

![Получение IPv6-адреса по DHCPv6 Stateful](image/20.png){ width=80% }

## Аренды DHCPv6 в Stateful-режиме

![Список аренд DHCPv6](image/21.png){ width=80% }

## Анализ трафика (Stateful DHCPv6)

![Анализ DHCPv6-пакетов в анализаторе трафика](image/22.png){ width=80% }

# Итоги работы

## Вывод

В ходе лабораторной работы:
- Развернут стенд в GNS3 с VyOS, коммутаторами и клиентами (VPCS и Kali Linux CLI).
- Настроен DHCP для IPv4:
  - автоматическая выдача адресов,
  - передача маски/шлюза/DNS/домена,
  - подтверждена корректность по статистике, арендам, журналу и анализу трафика.
- Реализованы два режима DHCPv6:
  - Stateless: адрес через SLAAC (RA), параметры через DHCPv6, без аренд адресов.
  - Stateful: адреса выдаются DHCPv6-сервером из диапазона, сервер ведёт учёт аренд.
- Анализ захваченного трафика подтвердил корректные сценарии DHCP, DHCPv6, RA и ICMPv6,
  соответствующие требованиям лабораторной работы.
