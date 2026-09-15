# 김원기 · Backend Developer

**업무의 흐름을 이해하고, 데이터로 개선하는 백엔드 개발자입니다.**

Java와 Spring Boot로 치료·상담 서비스 **Dr.CBT**의 백엔드를 개발하고 운영합니다.
예약부터 결제·환불·정산까지 복잡한 업무 규칙을 구현하고, 실행 로그로 성능 개선을 검증합니다.

[Portfolio](https://wongi-kim.github.io) · [Blog](https://velog.io/@wongi-kim/posts)

## Experience

**제이엔제이테크 · Dr.CBT 백엔드 개발·운영** · 2025.04 — 현재

백엔드 1인 담당으로 기능 개발, 운영 정책 반영, 조회 성능 개선을 맡고 있습니다.

- **예약·회기·워크북** — 예약 취소 후 회기 재배치, 행 잠금과 최초 제출 판정을 통한 중복 처리 방어
- **결제·환불·정산** — NICEPAY 온라인·링크·단말 결제 연동, 사용량 기반 환불 계산과 결제권 이력 관리
- **조회·운영** — 관리자 복합 조회, MySQL JSON 데이터 집계, AOP 공통 로깅과 파일 업로드·교체 처리

## Performance

반복 조회를 **배치 조회**로 바꾸고, **ID 기반 Map과 DTO 조립 구조**를 개선했습니다.

| 회원 목록 조회 | 평균 처리시간 | 감소율 |
| --- | ---: | ---: |
| 일반 회원 목록 | 249 → 67ms | **약 73%** |
| 담당 회원 목록 | 2,220 → 234ms | **약 89%** |

동일한 조회 조건의 변경 전후 실행 로그로 결과를 확인했습니다.
처리 흐름과 예외 조건, ERD도 문서화해 변경의 이유와 영향을 함께 남깁니다.

## Tech

| 구분 | 기술 |
| --- | --- |
| Backend | Java, Spring Boot, Spring Data JPA, QueryDSL, Spring Security |
| Data | MySQL, JSON 함수, Native Query |
| Operations & Test | Spring AOP, NCP Object Storage, GitHub Actions, JUnit 5, Mockito |
| Other projects | MongoDB, WebSocket, STOMP, RabbitMQ, Google Sheets API |

그 외 사용 경험: AWS, Docker, Redis

## Projects

### [Hot Item Collector](https://github.com/WonGi-Kim/hot-item-collector)

인기 아이템을 소개하고 거래하는 소셜 커머스 · 2024.07 — 2024.08

- IamPort(포트원) 결제 요청·검증·결과 처리와 Vue 화면 연동
- WebSocket·STOMP·RabbitMQ 채팅, MongoDB 메시지 저장, JWT 인증 컨텍스트 연결

### [PlayUs](https://github.com/WonGi-Kim/playus-backend)

사내 활동을 경험치로 기록하는 앱 · 두핸즈 × 블레이버스 공모전 · 2025.01

- Google Sheets와 서비스 DB의 데이터 연동·동기화
- MongoDB 하위 문서를 활용한 계정·활동 내역·연도별 경험치 포인트 모델링

## More

- [포트폴리오](https://wongi-kim.github.io) — 경력과 주요 프로젝트의 문제 해결 과정
- [기술 블로그](https://velog.io/@wongi-kim/posts) — 개발 과정에서 배운 내용과 기록
- [Dr.CBT](https://yd-icbt.co.kr) — 개발·운영 중인 치료·상담 서비스
