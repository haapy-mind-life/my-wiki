# API Design Hints

- REST/JSON API로 절차 트리거 (ex. `/api/v1/registration`)
- gRPC/Async API로 시뮬레이터와 연동
- 이벤트 브로커(Kafka/NATS)로 상태 변화 publish → 대시보드 소비

```http
POST /api/v1/pdu-sessions
Body: {"supi": "001010123456789", "dnn": "internet"}
```
