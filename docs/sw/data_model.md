# Data Model Ideas

- UE, Session, Policy, SecurityContext 등 주요 엔터티 정의
- ID/키: SUPI/SUCI, PDU Session ID, QoS Flow ID
- 저장소: 인메모리(개발용) → DB(운영) 확장 패턴

```yaml
UE:
  supi: string
  registration_state: enum
  sessions: [PduSession]
```
