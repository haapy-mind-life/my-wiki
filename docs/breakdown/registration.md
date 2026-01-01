# Registration Procedure (Simplified)

## 메시지 흐름
1. UE → AMF: Registration Request
2. AMF → AUSF: Authentication
3. AUSF → AMF: Authentication Response
4. AMF → UE: Security Mode Command & Complete
5. AMF ↔ SMF/PCF: 정책/세션 컨텍스트 준비
6. AMF → UE: Registration Accept/Complete

## 상태 전이 예시
- **INIT** → **AUTHENTICATING** → **SECURED** → **REGISTERED**
- 타이머: T3510, T3550, 재시도 횟수 관리

## 체크포인트
- UE 보안 모드 성공 여부
- NSSAI/TAI 유효성
- Emergency vs Normal 등록 구분
