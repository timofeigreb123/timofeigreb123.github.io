Тимофей Греб — Backend/Go разработчик
Делаю быстрые и надёжные сервисы под нагрузку, фокус на Go, PostgreSQL, Redis, Telegram Bot API, Docker/K8s.
Сайт: https://timofeigreb123.github.io · Email: you@example.com · Telegram: @yourhandle · GitHub: https://github.com/timofeigreb123

Быстрые ссылки
Проекты — см. ниже

Резюме — [ссылка на PDF/Notion]

Контакты — Email · Telegram · LinkedIn

Ключевые навыки
Языки: Go, Python (automation)

Хранилища: PostgreSQL, Redis

Инфра: Docker, Docker Compose, базовый Kubernetes, GitHub Actions

Практики: профилирование, p95/p99, observability (traces/metrics/logs), CI/CD, idempotency

Топ‑проекты
1) Realtime Leaderboard (Go + Redis)
Онлайн‑табло позиций игроков в реальном времени.

Роль: архитектура и backend, оптимизация Redis, деплой

Решения: Redis ZSET + Lua для атомарных апдейтов, батчи, graceful shutdown

Результат: p95 < 30 мс при 20k RPS, −25% CPU, 0 даунтайма за релиз

Стек: Go, Redis, Docker, Prometheus/Grafana

Ссылки: Live Demo · GitHub · Case/Документация

2) Telegram Bot Platform (Go + Postgres)
Платформа обработки 200k+ сообщений/сутки с очередями и ретраями.

Роль: проектирование схемы БД, консистентные ретраи, observability

Решения: idempotency ключи, circuit breaker, миграции, healthchecks

Результат: −40% p95, deliverability 99.7%

Стек: Go, PostgreSQL, Redis, tgbotapi, Docker

Ссылки: Live Demo · GitHub · Архитектура!
[дурка](https://github.com/user-attachments/assets/3234ec27-c7e9-4fd6-8fdb-f593fe541344)


3) TON USDT Validator (Go)
CLI/сервис для валидации адресов и статусов кошельков TON/USDT.

Роль: дизайн API, интеграции, тестирование

Решения: строгая валидация форматов, rate limit, кэширование

Результат: проверка 1k адресов < 2 с, покрытие тестами 85%

Стек: Go, HTTP client, Cobra/Viper, GitHub Actions

Ссылки: GitHub · README · Release

Избранные кейсы (подробности)
Highload оптимизация: снижение p95 на проде на 30–40% за счёт кеширования, батч‑обработки и профилирования CPU/allocs.

Надёжность: внедрение circuit breaker/retry/backoff, healthchecks и graceful shutdown для нулевого даунтайма релизов.

Наблюдаемость: метрики, трейсинг и структурные логи; дешёвая телеметрия для выявления деградаций до инцидента.
