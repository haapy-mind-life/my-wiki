# Mobility Management (Handover)

## 메시지 흐름 스케치
1. UE → gNB: Measurement Report
2. Source gNB → AMF/SMF: Handover Required/Request
3. Target gNB 준비 후: Handover Command
4. UE 동기화 → Path Switch → Release Resources

## 상태 전이
- **CONNECTED** → **HANDOVER_PREP** → **HANDOVER_EXEC** → **CONNECTED**
- 실패 시: **HANDOVER_FAILURE** 처리 후 재설정

## 체크포인트
- 측정 이벤트 (A3/A5 등) 트리거 조건
- 데이터 포워딩 여부 및 패킷 유실 최소화
- 타이머/가드 타임 관리
