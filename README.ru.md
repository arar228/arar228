<img src="assets/cover.svg" width="100%" alt="nepotato — продукты, инфраструктура и интерактивные системы" />

<p align="center">
  <a href="README.md">English</a> ·
  <a href="PROJECTS.md">Каталог проектов</a> ·
  <a href="docs/portfolio.ru.md">Подробные кейсы</a> ·
  <a href="https://github.com/arar228?tab=repositories">Репозитории</a> ·
  <a href="https://x.com/ton_potato">X / @ton_potato</a>
</p>

## Привет, я nepotato

Создаю веб-продукты, Telegram Mini Apps и инфраструктуру для их работы.
Соединяю **интерфейс, серверную логику и выпуск продукта**: React и TypeScript,
Python-автоматизацию, обработку данных и Linux-службы.

Использую AI-assisted development для перехода от идеи к коду, тестам и
развёртыванию. В репозиториях показываю инженерные решения, запускаемые примеры
и границы выполненной проверки.

## Избранные проекты

| Проект | Инженерный фокус | Посмотреть |
| :--- | :--- | :--- |
| **[Memora Solutions](https://github.com/arar228/memora-solutions)** | Web/desktop-инструменты, общий интерфейс, обработка платёжных событий и восстановление релиза | [Продукт](https://memorasolutions.ru) · [Архитектура](https://github.com/arar228/memora-solutions/blob/master/docs/architecture.md) |
| **[VPN Bridge](https://github.com/arar228/vpn-bridge-showcase)** | Защищённый маршрут через два узла, Hysteria2/REALITY, генерация конфигураций и оповещения | [Шифрование](https://github.com/arar228/vpn-bridge-showcase/blob/main/docs/security.md) · [Инженерный кейс](https://github.com/arar228/vpn-bridge-showcase/blob/main/docs/case-study.md) |
| **[RuMarket](https://github.com/arar228/rumarket-showcase)** | Сбор экономических данных, проверки качества и аналитический интерфейс с источниками | [Продукт](https://statik.obdrisher.ru/) · [Архитектура](https://github.com/arar228/rumarket-showcase/blob/main/docs/architecture.md) |
| **[Night Arcade](https://github.com/arar228/potato)** | Telegram Mini App, контракты API, виртуальный баланс и серверные игровые правила | [Инженерный кейс](https://github.com/arar228/potato/blob/main/docs/CASE_STUDY.md) |
| **[Procedural GPU](https://github.com/arar228/nepotato-threejs-gpu)** | Редактируемая Three.js-геометрия, переиспользуемый API и браузерное демо | [Открыть демо](https://arar228.github.io/nepotato-threejs-gpu/) |
| **[TON Subscriptions Protocol](https://github.com/arar228/ton-subscriptions-protocol)** | Исследование регулярных платежей, асинхронные переходы состояния и sandbox-тесты | [Контракты и тесты](https://github.com/arar228/ton-subscriptions-protocol) |

Memora и RuMarket содержат ссылки на продукты; статус и границы проверки описаны
в репозиториях. VPN Bridge — публичная очищенная версия частной инфраструктуры.
Night Arcade — прототип с игровыми очками. TON Subscriptions — исследовательские
контракты; работа с реальными средствами требует независимого аудита.

## Исследования и публикации

Публикую разборы исходного кода и on-chain-аналитику TON в
[@ton_potato](https://x.com/ton_potato). Избранные работы:

| Публикация | Исследовательский вклад | Источник |
| :--- | :--- | :--- |
| My Wallet · проверка NFT | Сравнение версий исходного кода и описание локальных тестов проверки владельца NFT перед подписанием | [Читать разбор](https://x.com/ton_potato/status/2107014919971361084) |
| Telegram Desktop · ссылки веб-входа | Разбор изменения безопасности: очистка login-токенов и различие между исправлением в исходном коде и выпущенной версией | [Читать разбор](https://x.com/ton_potato/status/2106795206397788169) |
| TON · предложение USDT | Сопоставление данных контракта и казначейства с отчётом эмитента; разделение обращения и резерва эмитента | [Читать разбор](https://x.com/ton_potato/status/2106409334619955430) |

Это самостоятельно опубликованные исследования. Исправления программ,
рассматриваемые в постах, реализованы разработчиками соответствующих проектов.

## Подход к разработке

**Продукт → контракты → реализация → проверка → выпуск.**

- Явное владение состоянием: контракты API, доступ и границы хранения.
- Восстановление после отказов: повторы, идемпотентные события, health checks и откат.
- Удобство ревью: команды запуска, описание архитектуры и воспроизводимые проверки.
- Описание безопасности через доверенные узлы и фактически используемые протоколы.

## Стек

**Интерфейс:** TypeScript, React, Vite, Tailwind CSS, Three.js.<br />
**Сервер и данные:** Node.js, Fastify, Python, PostgreSQL, Prisma, Zod, pandas.<br />
**Инфраструктура:** Linux, systemd, GitHub Actions, мониторинг и защищённые транспорты.

[Каталог публичных проектов](PROJECTS.md) включает интерфейсные эксперименты,
Telegram-инструменты, Python-упражнения и экосистемные работы.
[Подробное портфолио](docs/portfolio.ru.md) сохраняет развёрнутые описания кейсов.
