---
lang: ru-RU
title: "Отчёт по лабораторной работе 5"
subtitle: "Простые сети в GNS3. Анализ трафика"
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

Построение простейших моделей сети на базе коммутатора и маршрутизаторов FRR и VyOS в GNS3, анализ трафика посредством Wireshark.

# Выполнение лабораторной работы

## Справка по командам VPCS

![Просмотр списка команд VPCS](image/1.png){ #fig:001 width=80% }

## Справка по настройке IP

![Просмотр синтаксиса команды ip](image/2.png){ #fig:002 width=80% }

## Настройка IP-адреса PC1

![Настройка IP-адреса PC1 и проверка параметров](image/3.png){ #fig:003 width=80% }

## Проверка связности PC1 ↔ PC2

![Проверка связи между PC1 и PC2](image/4.png){ #fig:004 width=80% }

## ARP-сообщения (gratuitous ARP)

![Анализ ARP-сообщений в Wireshark](image/5.png){ #fig:005 width=80% }

## Опции ping в VPCS

![Просмотр параметров команды ping](image/6.png){ #fig:006 width=80% }

## Выполнение ping с PC2

![Выполнение ping](image/7.png){ #fig:007 width=80% }

## ICMP Echo Request/Reply

![Анализ ICMP Echo-запроса и ответа](image/8.png){ #fig:008 width=80% }

## UDP mode (Echo over UDP)

![Анализ UDP Echo-пакета](image/9.png){ #fig:009 width=80% }

## TCP mode (Echo over TCP)

![Анализ TCP-соединения и передачи данных](image/10.png){ #fig:010 width=80% }

## Топология: VPCS — Switch — FRR

![Топология сети с маршрутизатором FRR](image/11.png){ #fig:011 width=80% }

## Настройка IP на PC1 (192.168.1.10/24)

![Настройка IP-адреса PC1 и проверка параметров](image/12.png){ #fig:012 width=80% }

## Настройка eth0 на FRR (192.168.1.1/24)

![Настройка интерфейса eth0 маршрутизатора FRR](image/13.png){ #fig:013 width=80% }

## Проверка конфигурации FRR

![Проверка конфигурации и состояния интерфейсов маршрутизатора](image/14.png){ #fig:014 width=80% }

## Проверка связности PC1 → FRR (192.168.1.1)

![Проверка связи между PC1 и маршрутизатором](image/15.png){ #fig:015 width=80% }

## ICMP/ARP в Wireshark (PC1 ↔ FRR)

![Анализ ICMP-трафика между PC1 и маршрутизатором](image/16.png){ #fig:016 width=80% }

# Моделирование сети на базе VyOS

## Топология: VPCS — Switch — VyOS

![Топология сети с маршрутизатором VyOS](image/17.png){ #fig:017 width=80% }

## Настройка интерфейса eth0 на VyOS (192.168.1.1/24)

![Настройка интерфейса eth0 маршрутизатора VyOS](image/18.png){ #fig:018 width=80% }

## Проверка связности PC1 → VyOS (192.168.1.1)

![Проверка связи между PC1 и маршрутизатором VyOS](image/19.png){ #fig:019 width=80% }

## ICMP/ARP в Wireshark (PC1 ↔ VyOS)

![Анализ ICMP-трафика между PC1 и маршрутизатором](image/20.png){ #fig:020 width=80% }

# Выводы по работе

## Вывод

В ходе выполнения лабораторной работы были смоделированы простейшие сети в GNS3 на базе коммутатора Ethernet и маршрутизаторов FRR и VyOS. Выполнена статическая настройка IP-адресации в подсети 192.168.1.0/24 и проверена связность между узлами с использованием ICMP эхо-запросов.

С помощью Wireshark были захвачены и проанализированы ARP- и ICMP-сообщения, а также особенности формирования трафика при выполнении ping в режимах ICMP/UDP/TCP. Поставленные задачи выполнены в полном объёме.
