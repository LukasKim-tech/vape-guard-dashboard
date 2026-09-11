# 🛡 Vape Guard — 대시보드

ESP32 + SGP30 전자담배 감지 시스템의 웹 대시보드입니다.

**👉 https://lukaskim-tech.github.io/vape-guard-dashboard/**

## 처음 열었을 때

서버 주소 입력 화면이 뜹니다. Google Apps Script 배포 URL
(`https://script.google.com/macros/s/.../exec`)을 넣으면 연결됩니다.

입력한 주소는 **그 브라우저의 localStorage에만 저장**되며 어디로도 전송되지 않습니다.
이 저장소에는 서버 주소가 포함되어 있지 않습니다.

주소를 바꾸려면 우측 상단 ⚙ → **주소 변경**.

## 기능

- TVOC 실시간 표시 + 임계값 대비 게이지
- 최근 200개 측정 차트 (임계값 라인 + 알람 마커)
- 알람 시 사이렌 · 브라우저 알림 · 진동
- SYSTEM UPTIME 모니터링
- 원격 제어: 재시작 / 알림 테스트 / 기준값 리셋

## 소스

펌웨어·백엔드·3D 케이스를 포함한 전체 소스는 비공개 저장소에 있습니다.
이 저장소는 정적 대시보드 배포용입니다.
