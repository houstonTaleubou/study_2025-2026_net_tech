---
title: "Отчёт по лабораторной работе 7"
subtitle: "Адресация IPv4 и IPv6. Настройка DHCP"
author: "Талебу Тенке Франк Устон"
institute: "Российский университет дружбы народов"
email: "1032224534@pfur.ru"
lang: ru-RU
toc-title: "Содержание"
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl
toc: true
toc-depth: 2
lof: true
lot: false
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
polyglossia-lang:
  name: russian
  options:
    - spelling=modern
    - babelshorthands=true
polyglossia-otherlangs:
  name: english
babel-lang: russian
babel-otherlangs: english
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float}
  - \floatplacement{figure}{H}
---

![Топология лабораторного стенда в GNS3](image/1.png){ #fig:001 width=80% }

![Настройка IPv4-адреса интерфейса eth0](image/2.png){ #fig:002 width=80% }

![Настройка DHCP-сервера на VyOS](image/3.png){ #fig:003 width=80% }

![Получение IP-адреса по DHCP на PC1](image/4.png){ #fig:004 width=80% }

![Проверка IPv4-конфигурации и ping](image/5.png){ #fig:005 width=80% }

![Статистика DHCP-сервера](image/6.png){ #fig:006 width=80% }

![Журнал работы DHCP-сервера](image/7.png){ #fig:007 width=80% }

![Анализа DHCP](image/8.png){ #fig:008 width=80% }

![Расширенная топология лабораторного стенда](image/9.png){ #fig:009 width=80% }

![Настройка IPv6-адресов на интерфейсах VyOS](image/10.png){ #fig:010 width=80% }

![Настройка Router Advertisements и DHCPv6 Stateless](image/11.png){ #fig:011 width=80% }

![Просмотр конфигурации DHCPv4 и DHCPv6](image/12.png){ #fig:012 width=80% }

![Проверка IPv6-настроек на PC2](image/13.png){ #fig:013 width=80% }

![Ping IPv6-адреса маршрутизатора](image/14.png){ #fig:014 width=80% }

![Получение параметров по DHCPv6 Stateless](image/15.png){ #fig:015 width=80% }

![Состояние аренд DHCPv6](image/16.png){ #fig:016 width=80% }

![Анализ DHCPv6-пакетов в анализаторе трафика](image/17.png){ #fig:017 width=80% }

![Настройка DHCPv6 Stateful на VyOS](image/18.png){ #fig:018 width=80% }

![Начальные IPv6-настройки на PC3](image/19.png){ #fig:019 width=80% }

![Получение IPv6-адреса по DHCPv6 Stateful](image/20.png){ #fig:020 width=80% }

![Список аренд DHCPv6](image/21.png){ #fig:021 width=80% }

![Анализ DHCPv6-пакетов в анализаторе трафика](image/22.png){ #fig:022 width=80% }
