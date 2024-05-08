# Section2 API Gateway Service

## API Gateway
* 인증 및 권한 부여
* 서비스 검색 통합
* 응답 캐싱
* 정책, 회로 차단기 및 QoS 다시 시도
* 속도 제한
* 부하 분산
* 로깅, 추적, 상관 관계
* 헤더, 쿼리 문자열 및 청구 변환
* IP 허용 목록에 추가

### Netflix Ribbon
* Spring Cloud에서의 MSA간 통신
1. RestTemplate
   1. Web application에서 다른 Application에 사용하기 위한 템플릿
2. Feign Client
   1. 특정 인터페이스 생성 후, 추가 마이크로서비스 등록
   2. 자신이 가진 API 처럼 자유롭게 사용 가능

* Ribbon: Client side Load Balancer

-> 비동기 지원 불가능으로 잘 사용하지 않음

클라이언트 사이드에서 마이크로서비스를 로드 밸런서로 사용

-> ip:port 사용하지 않고 이름으로 호출 가능
1. 서비스 이름으로 호출
2. Health Check

### Netflix Zuul
* 구성
1. First Service
2. Second Service
3. Netflix Zuul

> Ribbon & zuul 모두 spring boot 2.4에서 maintenance 상태


