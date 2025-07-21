# Разработка концептуальной архитектуры.
## Cтек технологий для сервисов.

[Концептуальная_схема](./images/Концептуальная_схема.png)

### Мобильное приложение
  - **Платформы**: Android (Kotlin), iOS (Swift)
  - **Кросс-платформенный фреймворк**: React Native
  - **Состояние**: Redux
  - **Push-уведомления**: Firebase Cloud Messaging (FCM)
---
### Веб-интерфейс:
  - **Фронтенд-фреймворк**: React.js
  - **Аутентификация**: Keycloak (JWT)

---
### Telemetry Service
- **Язык**: Go
- **Очереди**: Kafka
- **Интеграции**: Garmin/HealthKit
- **База**: TimescaleDB

---
### Social Service
- **Язык**: Go
- **БД**: MongoDB 
- **Кеш**: Redis

---
### Training Service
- **Язык**: Java
- **Фреймворк**: Spring Boot
- **БД**: PostgreSQL

---
### Sale Service
- **Язык**: Java
- **Фреймворк**: Spring Boot
- **БД**: PostgreSQL
- **Кеш**: Redis

---
### User Service
- **Язык**: Java
- **Фреймворк**: Spring Boot + Spring Security
- **БД**: PostgreSQL
- **Интеграция**: Keycloak

--- 
### Catalog Service
- **Язык**: Go
- **БД**: Mongo
- **Кеш**: Redis

---
### Promo Service
- **Язык**: Java
- **Фреймворк**: Spring Boot
- **Геолокация**: Redis GEO
- **БД**: PostgreSQL

---
### Pay Service
- **Язык**: Java
- **Фреймворк**: Spring Boot
- **БД**: PostgreSQL

---

### Logistic Service

- **Язык**: Java
- **Фреймворк**: Spring Boot
- **БД**: PostgreSQL

--- 
###  Вспомогательные системы

- **Кеширование**: Redis
- **Хранилище файлов**: MinIO
- **Мониторинг**:
    - Java: Micrometer + Prometheus
    - Go: Prometheus client_golang
- **Оркестрация**: Kubernetes
- **Очереди**: Kafka


