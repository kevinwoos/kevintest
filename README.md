# kevintest
MSA의 핵심 원칙
- Componentization via Services : 서비스를 통한 구성 요소화
- Organized around Business Capabilities : 비즈니스 역량을 중심으로 조직 구성
- Products not Projects : 프로젝트가 아닌 제품
- Smart endpoints and dumb pipes : 스마트 엔드포인트와 멍청한 파이프
- Decentralized Data Management / Governance : 분산형 데이터 관리/거버넌스
- Infrastructure Automation : 인프라 자동화
- Design for Failrue : 실패를 위한 설계
- Evolutionary Design : 진화적 설계

Conway's Law : 시스템이 설계되면, 그 시스템의 구조는 설계한 조직의 구조와 유사해진다.
- Business Capabailities : 조직이 얼마나 빠르고 유연하게 변화에 대응할 수 있는지에 대한 능력

- https://microservices.io/index.html
- MSA 이론 정리 : https://it-noongam.tistory.com/20
- DDD : https://happycloud-lee.tistory.com/94 , https://velog.io/@suhongkim98/MSA%EC%99%80-DDD-%EB%8F%84%EB%A9%94%EC%9D%B8-%EC%A3%BC%EB%8F%84-%EC%84%A4%EA%B3%84%EB%9E%80-2

ㅇ 필요성의 측면에서의 자가진단
- 개발, 배포 시 다른 팀의 소스 혹은 공통 모듈 등으로 인한 일정 조율/커뮤니케이션이 방해될 정도인가요?
- 느려지는 개발, 배포 과정으로 인해 필요한 비즈니스 개발이 지연된 적이 있나요 ? (Business Capabilities)
- 단 건의 배포로 인한 전체적인 영향도 파악이 어렵고, 실제로 이로 인해 놓친 부분으로 인해 장애가 빈번하게 발생하나요 ?
- 공통적으로 사용하는 모듈 수정 시, 영향도 파악과 커뮤니케이션에 대한 부담이 압박으로 다가오나요 ?
- 주요 서비스로 인한 빈번한 DB 부하로 인해, 타 서비스에서 영향을 받은 적이 빈번한가요?

ㅇ 가능 여부 측면에 대한 자가진단
- 엔지니어링 조직에서 MSA 구조와 각 서비스의 통신에 대한 기본적인 아키텍처를 이해하고 있나요 ?
- CI/CD 파이프라인을 위한 Devops/SRE 조직이 별도로 존재하고 트러블 슈팅을 위한 인프라 지식이 있나요 ?
- 어려워진 트러블슈팅과 모니터링 난이도를 해결하기 위한 스택(EFK, Prometheus, Elastic Search, Grafana, ... ) 들 구축을 적절하게 할 수 있는 상황인가요 ?
- MSA/Cloud 환경에 대한 적절한 보안을 책임질 수 있는 보안 담당자가 존재하나요?
- 사내 엔지니어링 최고 책임자가 MSA 전환에 대한 충분한 필요성을 느끼고 공감하나요?

ㅇ Lesson-Learn
- 성급한 세분화
- Business Capabilities 가 비교적 덜 필요한 경우
- 적절한 팀 내 프로세스와 문화, 스킬들의 보유
......
무엇보다,, 현 상황에 대한 다양한 기술들의 적용들에 있어서 Why 에 대한 Because 를 자신있게 말할 수 있다면..!
