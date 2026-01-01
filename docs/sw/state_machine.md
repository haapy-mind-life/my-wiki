# State Machine Examples

## Registration State Machine
- INIT → AUTHENTICATING → SECURED → REGISTERED
- Failure → RETRY/ABORT 경로 포함

## Session State Machine
- IDLE → SESSION_PENDING → ACTIVE → RELEASED
- QoS 업데이트/타이머 이벤트를 트리거로 상태 전이
