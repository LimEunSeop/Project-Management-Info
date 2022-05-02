# Project-Management-Info
프로젝트 관리 공부

## 기획

- 기능명세서, 와이어프레임: [https://velog.io/@vonvoyage27/포트폴리오-멘토링-두번째-수업-회고-기능-명세서-UI-기획서](https://velog.io/@vonvoyage27/%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4-%EB%A9%98%ED%86%A0%EB%A7%81-%EB%91%90%EB%B2%88%EC%A7%B8-%EC%88%98%EC%97%85-%ED%9A%8C%EA%B3%A0-%EA%B8%B0%EB%8A%A5-%EB%AA%85%EC%84%B8%EC%84%9C-UI-%EA%B8%B0%ED%9A%8D%EC%84%9C)  ⇒ 피그마 사용하자 그냥
- DB 모델링: SQL vs NoSQL
- 디자인 시스템 정의 (약식으로, Figma 를 사용할 줄 알면 좋겠으나 시간이 부족하면 코딩으로 쳐보고 임포트하도록)

## 개발

### language

HTML, CSS, ES6+, Typescript

### skills

해당 항목들을 면밀히 따져보며 프로젝트 실정에 맞게 객관성에 근거한 주관적인 안목으로 잘 선택할 것.

- Front-end: React, (rxJS)
- Styling: CSS-in-JS vs CSS-in-CSS
- State Management: Mobx vs Recoil
- Back-end: Firebase or (Nest.js vs Express.js, Prisma ...)
- DB: PostgreSQL vs MongoDB

### Work Flow

- 기획 산출물: 노션에 작성 및 기타 링크 첨부
- API 문서(if backend): swagger autogen 사용
- 데이터 구조(if serverless): 관련 기술 뭐가 있는지 찾아봐야됨
- 업무 할당: GIthub Issue 사용
- 메신저: Slack
- Slack 채널 연동할것: 좀 더 조사 필요
- 개발 방법론: 비즈니스 로직은 TDD, UI 관련한 것은 완성후 스냅샷 테스팅 & 콜백 호출 테스트, 마지막 통합테스트
- 할당 방식: 내가 먼저 테스트코드 작성하고 팀원에게 전달할까 생각중
- 프로젝트 진행 방식: 주 2회(월목, 화금) 만나서 코드리뷰 및 다음 진행할것 회의, 남는시간 코딩. 집에서 주로 코딩하고 회의 내용을 기반으로
- 기술교육: 팀원이 처음 접하는 기술이다 싶으면 샘플 몇개 작성해서 던져주고 익숙해지도록. 관련된 문서 찾아서 주며 시간 점점 줄여나가도록
- 회의록 작성하기: 회의록 협업에 대한 중요성 기록, 기술적인 깨달음, 갈등 대처 방식 등등..

## 인프라

- CI/CD pipeline: CircleCI ... 등등 서비스 찾아보기
- Docker Container: 사용하는게 나을까? 나중에 도입해도 좋을듯.
- Server: Netlify, AWS .... 뭘 사용해야 될까?
- Storage Service
- 또 뭐가 있을까? 내일은 이쪽을 좀 더 살펴봐야겠다.
