[언어 선택으로 돌아가기](../../README.md)

# Corellium에 Dopamine 설치하기

1. endpoint.sample.json을 endpoint.json으로 복사하고 Corellium 계정 자격 증명을 추가합니다. 사용자 이름+비밀번호 조합 또는 totp 토큰 중 하나가 필요합니다.
2. Dopamine을 컴파일합니다.
3. `codesign -dvvvv on BaseBin/dopamine/dopamine`를 실행합니다.
4. CandidateCDHash를 복사하여 비탈옥된 Corellium 인스턴스의 Settings -> Trust Cache에 붙여넣습니다.
5. `env NODE_TLS_REJECT_UNAUTHORIZED=0 node dopamine.js install <Project> <Instance>`를 실행합니다. `Project`와 `Instance`는 이름 또는 ID일 수 있습니다.
6. 인스턴스의 "Port Forwarding"에서 포트를 추가합니다: Device port = 22, Router port = 22, expose port 활성화
7. 장치가 Wi‑Fi 네트워크에 연결되어 있는지 확인합니다.
8. "Connect"에서 하단에 Wi‑Fi IP를 확인할 수 있습니다.
9. 이제 `ssh mobile@<Wi-Fi IP>`로 장치에 SSH 접속할 수 있습니다.

---
번역: 기계 번역 + GitHub Copilot Chat Assistant 교정
