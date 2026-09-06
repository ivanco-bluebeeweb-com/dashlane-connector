# Dashlane Connector — Auth & Credentials Standard

**Compliance:** AUTH_AND_CREDENTIALS_STANDARD.md (B1–B10)

## Схема аутентификации
- **Метод:** Dashlane Business API Key + Master Access Token
- **Хранение:** Секреты сохраняются изолированно в хранилище секретов платформы Imperal.
- **Валидация:** При сохранении ключа выполняется тестовый запрос `GET /v1/team/members`.
- **Отключение:** Удаление локальных ключей без воздействия на аккаунт вендора.
