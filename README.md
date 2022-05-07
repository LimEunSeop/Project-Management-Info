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
- Testing: Jest, Jest-dom, React Testing Library, Cypress, Cypress Testing Library

### Work Flow

- 기획 산출물: 노션에 작성 및 기타 링크 첨부
- API 문서(if backend): swagger autogen 사용
- 데이터 구조(if serverless): 관련 기술 뭐가 있는지 찾아봐야됨
- 업무 할당: GIthub Issue 사용
- 메신저: Slack
- Slack 채널 연동할것: 좀 더 조사 필요
- 개발 방법론: 비즈니스 로직은 TDD, UI 관련한 것은 완성후 스냅샷 테스팅 & 콜백 호출 테스트, 마지막 통합테스트
- 할당 방식: 내가 먼저 테스트코드 작성하고 팀원에게 전달할까 생각중
- 프로젝트 진행 방식: 주 2회(월목, 화금) 만나서 코드리뷰 및 다음 진행할것 회의, 남는시간 코딩. 집에서 주로 코딩하고 회의 내용을 기반으로 테스트코드 미리 작성해두기
- 기술교육: 팀원이 처음 접하는 기술이다 싶으면 샘플 몇개 작성해서 던져주고 익숙해지도록. 관련된 문서 찾아서 주며 시간 점점 줄여나가도록
- 회의록 작성하기: 회의록 협업에 대한 중요성 기록, 기술적인 깨달음, 갈등 대처 방식 등등..

## 인프라

일단 소스가 올라갈 서버가 있어야 하고, CI/CD 파이프라인 갖추고, 첨부파일 관리할 서버가 따로 필요할듯.

- CI/CD pipeline: CircleCI ... 등등 서비스 찾아보기
- Docker Container: 사용하는게 나을까? 나중에 도입해도 좋을듯.
- Server: Netlify, AWS .... 뭘 사용해야 될까?
- Storage Service
- 또 뭐가 있을까? 내일은 이쪽을 좀 더 살펴봐야겠다.
- Backend: Firebase를 쓸까 AWS Lambda를 쓸까

## 토이프로젝트 인사이트 얻을 수 있는곳

- [https://devfolio.kr](https://devfolio.kr/) : 토이프로젝트 모아보기 서비스
- [https://bside.best](https://bside.best/), [https://www.depromeet.com](https://www.depromeet.com/) : 팀 빌딩 사이트

## 다음 할 일

1. 너무 중구난방으로 정리해서 뭘 수집해야될지 모르겠다.. 다시 정신차리고 살펴보자. 기획, 저정도면 괜찮고 skills도 저정도면 괜찮음. 
2. 다만 work flow 섹션에서 slack 관련 연동 정보가 아직 미비되었고, 프로젝트 상태를 나타내기 위한 Dashboard 가 부족하다. 인프라는 더욱이 그림이 안 잡힌다.
3. 프로젝트 slack 연동 정보 찾기 - Git commit 알림, CI/CD 파이프라인 Status 정도 알리는 기능이면 충분할듯. 나중에 더 필요하면 붙여 나가는 식으로 하자
4. 프로젝트 상태 관련 대쉬보드 중 CI Status 는 [여기](https://github.com/cypress-io/cypress-example-kitchensink) 를 참고하나, 일단은 프로젝트를 진행하면서 진정 필요한게 뭔지 느끼는 시간을 가지면 될듯 하다. - github [README.md](http://README.md) 에 딱히 상태를 관리할 필요는 없는듯 하다. 프로젝트 참여자들 끼리 slack 채널에서 보이도록 하기만 하면 충분하지 않을까? 아니다. 그래도 slack 에서 본다면 알림으로서는 충분하지만 대쉬보드로서의 기능이 떨어질것 같음.. 프로젝트에 관여하는 플랫폼으로의 링크를 README.md 에 표시하면 난 좋을것 같다. README.md 에 대쉬보드로서 한눈에 전체 프로세스를 볼 수 있도록 하고 클릭하면 그 플랫폼의 상세를 볼 수 있도록.
5. ~~정리된 work flow 를 바탕으로 진짜 루틴하게 효율적으로 일 할 수 있는 순서를 어느정도 구상해 놓아야 될듯 싶다. 진짜 말로만 열심히 한다 자신하는 구조가 아닌, 어느 누구라도 부담없이 일에 집중할 수 있는 구조로.~~
6. 인프라 관련해서는 다시한번 여러 블로그나 [https://devfolio.kr](https://devfolio.kr/) 돌아다니면서 수집해보도록 하자. 규모는 작을지언정 역할분리의 측면에서 나름 현업에 견줄만하게 준수한 정도였으면 좋겠다. - Storage Service: [Amazon S3](https://aws.amazon.com/ko/s3/), [Cloudinary](https://cloudinary.com). API Server: AWS API Gateway, [AWS Lambda](https://aws.amazon.com/ko/lambda/), [AWS EC2 vs AWS Lightsail](https://devlog.jwgo.kr/2020/06/21/ec2-vs-lightsail/), DB: NoSQL([AWS DynamoDB vs AWS DocumentDB](https://jane-aeiou.tistory.com/57)), RDB([AWS RDS](https://us-west-2.console.aws.amazon.com/rds/home?region=us-west-2)). 프론트엔드 서비스 방법은?? 
7. 프론트엔드를 AWS Lambda에 배포하는 방법, CI/CD 파이프라인 구축방법 찾기

정보수집 중 남는시간이 있으면 Mobx 후다닥 공부하기~
