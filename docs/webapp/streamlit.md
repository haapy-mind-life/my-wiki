# Streamlit Prototype

- 입력: SUPI, 절차 타입 (Registration/PDU Session)
- 출력: 상태 전이 그래프, 메시지 타임라인
- 옵션: 시나리오 스크립트 업로드 → 시뮬레이션 실행

```python
import streamlit as st

supi = st.text_input("SUPI")
procedure = st.selectbox("Procedure", ["Registration", "PDU Session"])
st.write("Run simulation for", supi, procedure)
```
