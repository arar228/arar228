<img src="assets/cover.svg" width="100%" alt="nepotato — full-stack разработка. Интерфейсы, системы, выпуск продукта." />

[English](README.md) · [Memora](https://memorasolutions.ru) · [RuMarket](https://statik.obdrisher.ru/) · [Репозитории](https://github.com/arar228?tab=repositories)

[Каталог публичных проектов](PROJECTS.md) — продуктовые кейсы, frontend-эксперименты,
Telegram-инструменты, учебные работы и участие в экосистеме.

Разрабатываю веб-продукты, Telegram Mini Apps и интерактивные инструменты. В проектах соединяю **React-интерфейс, серверную логику и хранение данных** с тестами и процессом выпуска.

## Портфолио проектов

### Memora Solutions

**Продуктовая платформа · React / Node.js / PostgreSQL / Python / Electron**

Набор инструментов для работы и повседневных задач: web/desktop Pomodoro, поиск туристических предложений, Kanban и Telegram-интеграции.

- Общий интерфейс Pomodoro с отдельными адаптерами хранения для браузера и desktop.
- Проверка платёжных событий, идемпотентная отправка и восстановление после сбоев в Travel Radar.
- Выпуск точного commit SHA, проверка состояния и откат приложения на VPS.

[Открыть продукт](https://memorasolutions.ru) · [Код](https://github.com/arar228/memora-solutions) · [Архитектура](https://github.com/arar228/memora-solutions/blob/master/docs/architecture.md) · [CI](https://github.com/arar228/memora-solutions/actions/workflows/ci.yml)

### Night Arcade

**Full-stack прототип · TypeScript / React / Fastify / Prisma / PostgreSQL**

Telegram Mini App с виртуальными игровыми очками, журналом операций, ежедневными наградами и игровыми раундами с серверным определением результата. Репозиторий опубликован под именем `potato`.

- Общие Zod-контракты связывают интерфейс и API.
- Сервер управляет балансом и результатом игры; клиент отвечает за отображение.
- Unit-тесты проверяют игровые правила, авторизацию и сервис кошелька с подменённым хранилищем.

**Границы:** прототип с игровыми очками. PvP — демонстрация с Arcade Bot; полноценный мультиплеер и готовность к реальным платежам требуют отдельной проверки и доработки.

[Код и запуск](https://github.com/arar228/potato) · [Инженерный кейс](https://github.com/arar228/potato/blob/main/docs/CASE_STUDY.md)

### Procedural GPU

**Интерактивная графика · TypeScript / Three.js / WebGL**

Редактируемая модель трёхвентиляторной видеокарты из процедурной геометрии. Переиспользуемый API модели дополнен интерактивным браузерным демо.

<a href="https://arar228.github.io/nepotato-threejs-gpu/"><img src="https://raw.githubusercontent.com/arar228/nepotato-threejs-gpu/main/docs/preview.png" width="640" alt="Процедурная модель видеокарты; открыть интерактивное демо" /></a>

[Открыть демо](https://arar228.github.io/nepotato-threejs-gpu/) · [Код и API](https://github.com/arar228/nepotato-threejs-gpu)

### RuMarket

**Экономическая аналитика · Python / pandas / NumPy / SciPy / JavaScript**

Объяснимый автоматически обновляемый монитор экономики России и финансовых рынков. Он объединяет официальную статистику, рыночные цены, кредитные условия и корпоративную отчётность в интерфейсе с указанием источников.

- Автоматический сбор данных Московской биржи, Банка России, Росстата и Минфина.
- Проверки актуальности, покрытия, допустимых диапазонов и обязательных бюджетных показателей.
- Обновления по расписанию, снимки состояния, последняя успешная версия данных и проверки восстановления публикации.

[Открыть продукт](https://statik.obdrisher.ru/) · [Инженерный кейс](https://github.com/arar228/rumarket-showcase) · [Архитектура](https://github.com/arar228/rumarket-showcase/blob/main/docs/architecture.md)

### TON Subscriptions Protocol

**Контрактная логика · Tolk / TypeScript / TON Sandbox**

Исследовательский проект регулярных платежей: детерминированные адреса, переходы состояния по времени, пауза и возобновление подписки, тесты возврата отклонённых переводов.

**Границы:** публичный репозиторий содержит контракты и sandbox-тесты. Для реальных средств требуется независимый аудит безопасности; отдельные прикладные сервисы находятся за пределами этого репозитория.

[Код и архитектура](https://github.com/arar228/ton-subscriptions-protocol) · [Sandbox-тесты](https://github.com/arar228/ton-subscriptions-protocol/tree/master/tests)

## Решения, которые стоит посмотреть

| Вопрос | Пример в коде и документации |
| --- | --- |
| Как общий интерфейс работает с разным хранением в web и desktop? | [Карта компонентов Memora](https://github.com/arar228/memora-solutions/blob/master/docs/component-map.md) |
| Как устроены повтор платёжного запроса и откат релиза? | [Эксплуатация Memora](https://github.com/arar228/memora-solutions/blob/master/docs/operations.md) |
| Какие правила принадлежат серверу? | [Кейс Night Arcade](https://github.com/arar228/potato/blob/main/docs/CASE_STUDY.md) |
| Как аналитический конвейер показывает качество и актуальность источников? | [Архитектура RuMarket](https://github.com/arar228/rumarket-showcase/blob/main/docs/architecture.md) |
| Что происходит при возврате асинхронного перевода? | [Тесты bounce-сценариев](https://github.com/arar228/ton-subscriptions-protocol/blob/master/tests/ChannelJettonBounce.spec.ts) |

## Стек проектов

**Интерфейс** — TypeScript, React, Vite, Tailwind CSS, Three.js<br>
**Сервер и данные** — Node.js, Fastify, Python, PostgreSQL, Prisma, Zod, pandas, NumPy, SciPy<br>
**Выпуск и проверка** — GitHub Actions, unit-тесты, воспроизводимые сборки, health checks

В каждом репозитории указаны команды запуска и границы проверки. Опубликованные продукты, локальные прототипы и контрактные эксперименты имеют отдельные обозначения статуса.
