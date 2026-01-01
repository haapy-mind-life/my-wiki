# PDU Session Establishment (Overview)

## 메시지 흐름
1. UE → AMF: PDU Session Establishment Request
2. AMF → SMF: PDU Session Create (Nsmf_PDUSession)
3. SMF → UPF: Session Setup (N4)
4. SMF → AMF → UE: PDU Session Accept

## 상태 전이 예시
- **IDLE** → **SESSION_PENDING** → **ACTIVE**
- QoS/NSSAI 매핑 및 정책 제어 포인트

## 체크포인트
- DNN/S-NSSAI 유효성
- IPv4/IPv6 주소 할당 여부
- QoS Flow / PDR 생성 결과
