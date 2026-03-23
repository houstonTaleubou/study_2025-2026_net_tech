---
title: "Отчёт по лабораторной работе 8"
subtitle: "Адресация IPv4 и IPv6. Настройка маршрутизации"
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
![Топология сети в GNS3](image/1.png){ #fig:001 width=80% }

![Настройка IPv6 на PC1](image/2.png){ #fig:002 width=80% }

![Настройка IPv6 на PC2](image/3.png){ #fig:003 width=80% }

![Изменение имени и подготовка gw-01](image/4.png){ #fig:004 width=80% }

![Настройка интерфейсов gw-01](image/5.png){ #fig:005 width=80% }

![Изменение имени gw-02](image/6.png){ #fig:006 width=80% }

![Настройка интерфейсов gw-02](image/7.png){ #fig:007 width=80% }

![Изменение имени gw-03](image/8.png){ #fig:008 width=80% }

![Настройка интерфейсов gw-03](image/9.png){ #fig:009 width=80% }

![Проверка IPv6 на PC1](image/10.png){ #fig:010 width=80% }

![Проверка IPv6 на PC2](image/11.png){ #fig:011 width=80% }

![Проверка связности с gw-01](image/12.png){ #fig:012 width=80% }

![Анализ трафика между маршрутизаторами](image/13.png){ #fig:013 width=80% }

![Настройка RIP на gw-01](image/14.png){ #fig:014 width=80% }

![Настройка RIP на gw-02](image/15.png){ #fig:015 width=80% }

![Настройка RIP на gw-03](image/16.png){ #fig:016 width=80% }

![Проверка связности после настройки RIP](image/17.png){ #fig:017 width=80% }

![Анализ трафика ICMP и RIP](image/18.png){ #fig:018 width=80% }

![Настройка туннеля на gw-01](image/19.png){ #fig:019 width=80% }

![Настройка туннеля на gw-02](image/20.png){ #fig:020 width=80% }

![Статический IPv6-маршрут на gw-01](image/21.png){ #fig:021 width=80% }

![Статический IPv6-маршрут на gw-02](image/22.png){ #fig:022 width=80% }

![Проверка связности с PC1](image/23.png){ #fig:023 width=80% }

![Проверка связности с PC2](image/24.png){ #fig:024 width=80% }

![Общий вид трафика IPv6](image/25.png){ #fig:025 width=80% }

![Структура инкапсулированного пакета](image/26.png){ #fig:026 width=80% }

