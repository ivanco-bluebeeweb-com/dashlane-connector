# Dashlane Connector — Connector Discovery

**Official Documentation:** https://dashlane.com  
**Base URL:** https://business-api.dashlane.com/v1  
**Auth Model:** Dashlane Business API Key + Master Access Token  

## Основные сущности вендора
- пользователи команды (/users), индекс безопасности (security score), аудит событий (/audit-logs)

## Лимиты и особенности API
- Соблюдение Rate Limits вендора, обработка HTTP 429 с экспоненциальным backoff.
- Валидация входных данных по Pydantic-схемам вендора до отправки запроса.
- Тестовая точка проверки подключения: `GET /v1/team/members`.
