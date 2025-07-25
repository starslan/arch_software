## ADR 3: Выбор обработчика событий
**Дата:** 2025-07-18  
**Статус:** Принято

### Контекст
Обработка потоковых данных с IoT-устройств (10K+ событий/сек).

### Сравнение вариантов
| Критерий          | Apache Kafka     | RabbitMQ         | **Выбор**        |
|-------------------|------------------|------------------|------------------|
| **Пропускная способность** | 1M+ сообщ/сек | 50K сообщ/сек    | **Kafka**  |
| **Задержка**      | < 10 мс          | < 5 мс           | —                |
| **Надёжность**    | Репликация       | Очереди          | **Kafka**        |
| **Сложность**     | Высокая          | Низкая           | —                |

### Решение
Apache Kafka.

### Обоснование
Соответствие НФТ по масштабируемости для сценариев соревнований.

### Последствия
- Поддержка пиковых нагрузок до 10K участников
- Рост затрат на инфраструктуру
- Необходимость выделенного кластера