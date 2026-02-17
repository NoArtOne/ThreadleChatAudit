# Зависимости проекта
| Библиотека                                         | Назначение                                   | Документация                                                                                                           |
|----------------------------------------------------|----------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| github.com/go-telegram-bot-api/telegram-bot-api/v5 | Клиент для Telegram Bot API                  | [Docs](https://pkg.go.dev/github.com/go-telegram-bot-api/telegram-bot-api/v5?spm=a2ty_o01.29997173.0.0.25485171XLlhBX) |
| modernc.org/sqlite                                 | Драйвер SQLite (pure Go, без CGO)            | [Docs](https://pkg.go.dev/modernc.org/sqlite?spm=a2ty_o01.29997173.0.0.25485171XLlhBX)                                 |
| github.com/joho/godotenv                           | Загрузка переменных окружения из .env        | [Docs](https://pkg.go.dev/github.com/joho/godotenv?spm=a2ty_o01.29997173.0.0.25485171XLlhBX)                           |                                                                                                         |
| github.com/robfig/cron/v3                          | Планировщик задач (для авто-саммари в 08:00) | [Docs](https://pkg.go.dev/github.com/robfig/cron/v3?spm=a2ty_o01.29997173.0.0.25485171XLlhBX)                          |
## Внешние сервисы llama.cpp (Docker)
Локальный LLM-сервер с OpenAI-compatible API
Запускается отдельно, порт 8080
## Установка зависимостей
```bash
go mod tidy
```
## Быстрый старт
1. Скопируйте .env.example в .env и заполните токены.
2. Запустите llama.cpp через Docker:
```bash
docker-compose up -d
```
3. Запустите бота:
```bash
go run cmd/bot/main.go
```
