스프링 부트 참고가이드
=====================

# 작성자
Phillip Webb, Dave Syer, Josh Long, Stéphane Nicoll, Rob Winch, Andy Wilkinson, Marcel Overdijk, Christian Dupuis, Sébastien Deleuze

1.2.0.BUILD-SNAPSHOT

Copyright © 2013-2014

Copies of this document may be made for your own use and for distribution to others, provided that you do not charge any fee for such copies and further provided that each copy contains this Copyright Notice, whether distributed in print or electronically.

*****

# I. 스프링부트 문서
## 1. 문서에 대해
## 2. 도움 구하기
## 3. 첫걸음
## 4. 스프링부트 작동
## 5. 스프링부트 기능 학습
## 6. 출시
## 7. 고급주제

# II. 시작
## 8. 스프링부트 시작
## 9. 시스템 요구사항
### 9.1. 서블릿 컨테이너
## 10. 스프링부트 설치
### 10.1. 자바 개발자를 위한 설치법 소개
#### 10.1.1. 메이븐 설치
#### 10.1.2. 그레들 설치
### 10.2. 스프링부트 CLI를 이용한 설치
#### 10.2.1. 메뉴얼 설치법
#### 10.2.2. GVM을 이용한 설치법
#### 10.2.3. OSX Homebrew 설치법
#### 10.2.4. 커맨드라인 완성
#### 10.2.5. 스프링 CLI로 빠르게 시작하는 예제
### 10.3. 이전버전의 스프링부트로부터 업그레이드
## 11. 초기 스프링부터 애플리케이션 개발
### 11.1. POM 파일 생성
### 11.2. classpath 의존성 추가
### 11.3. 코드 작성
#### 11.3.1. ```@RestController```와 ```@RequestMapping``` 애노테이션
#### 11.3.2. ```@EnableAutoConfiguration``` 애노테이션
#### 11.3.3. "main" 메서드
### 11.4. 예제 실행
### 11.5. 실행가능한 jar 생성
## 12. 다음 읽을거리

# III. 스프링부트 사용<a name="III. 스프링부트 사용"></a>
## 13. 빌드 시스템
### 13.1. 메이븐
#### 13.1.1. 스프링부트 스타터 부모 상속
#### 13.1.2. 부모 POM 없이 스프링부트 사용
#### 13.1.3. 자바 버전 변경
#### 13.1.4. 스프링부트 메이븐 플러그인 사용
### 13.2. 그레들
### 13.3. 앤트
### 13.4. 스프링부트 스타터 POM 목록
## 14. 코드 구성하기
### 14.1. 'default' 패키지 이용
### 14.2. 메인 애플리케이션 클래스 위치
## 15. 설정 클래스들
### 15.1. 추가된 설정 클래스들 불러오기
### 15.2. XML 설정 불러오기
## 16. 자동설정(Auto-configuration)
### 16.1. 점진적으로 자동설정을 대체
### 16.2. 특정한 자동설정을 비활성화
## 17. 스프링 빈과 의존성 주입
## 18. ```@SpringBootApplication```애노테이션 사용
## 19. 애플리케이션 실행
### 19.1. IDE에서 실행
### 19.2. 패키징된 애플리케이션 실행
### 19.3. 메이븐 플러그인 이용
### 19.4. 그레들 플러그인 이용
### 19.5. 핫스와핑
## 20. 출시를 위한 애플리케이션 패키징
## 21. 다음 읽을거리

# IV. 스프링부트 기능
## 22. 스프링애플리케이션
### 22.1. 배너 수정
### 22.2. 스프링애플리케이션 수정
### 22.3. 플루언트 빌더 API
### 22.4. 애플리케이션 이벤트와 리스너
### 22.5. 웹 환경
### 22.6. 커맨드라인러너 사용
### 22.7. 애플리케이션 종료
## (23. 외부설정)[#23. 외부설정]
### 23.1. 커맨드라인 속성 접근
### 23.2. 애플리케이션 속성 파일들
### 23.3. 프로파일 지정 속성들
### 23.4. 속성 플레이스홀더(placeholder)
### 23.5. Properties 대신 YAML 사용
#### 23.5.1. YAML 읽어오기
#### 23.5.2. 스프링 환경에서 속성들을 YAML로 노출
#### 23.5.3. 다중 프로파일 YAML 문서
#### 23.5.4. YAML 의 단점
### 23.6. 타입세이프 설정 속성들
#### 23.6.1. 느슨한 연결
#### 23.6.2. ```@ConfigurationProperties``` 검증
## 24. 프로파일
### 24.1. 활성프로파일 추가
### 24.2. 프로파일 작성방법
### 24.3. 프로파일 상세 설정파일
## 25. 로깅
### 25.1. 로그 형식
### 25.2. 콘솔 출력
### 25.3. 파일 출력
### 25.4. 로그 레벨
### 25.5. [로그 설정 변경](#로그 설정 변경)
## 26. 웹 애플리케이션 개발
### 26.1. 'Spring Web MVC framework'
#### 26.1.1. Spring MVC 자동설정
#### 26.1.2. ```HttpMessageConverter```
#### 26.1.3. ```MessageCodesResolver```
#### 26.1.4. ```Static Content````
#### 26.1.5. Template engines
#### 26.1.6. 오류 제어, 웹스피어
#### 애플리케이션 서버에서 오류 제어
### 26.2. JAX-RS 그리고 Jersey
### 26.3. 내장형 서블릿 컨테이너 지원
#### 26.3.1. 서블릿 그리고 필터
#### 26.3.2. ```EmbeddedWebApplicationContext```
#### 26.3.3. 내장형 서블릿 컨테이너 변경
#### 변경 작성방법
#### ```ConfigurableEmbeddedServletContainer``` 직접 변경
#### 26.3.4. JSP 제약사항
## 27. 보안
## 28. SQL 데이터베이스 작업
### 28.1. 데이터베이스 설정
#### 28.1.1. 내장형 데이터베이스 지원
#### 28.1.2. 외부 데이터베이스 연결
#### 28.1.3. JNDI 데이터베이스 연결
### 28.2. JdbcTemplate 사용
### 28.3. JPA 그리고 'Spring Data'
#### 28.3.1. 엔티티 클래스
#### 28.3.2. Spring Data JPA 레파지토리
#### 28.3.3. JPA 데이터베이스 생성 및 삭제
## 29. NoSQL 기술 작업
### 29.1. 레디스Redis
#### 29.1.1. 레디스 연결
### 29.2. 몽고DBMongoDB
#### 29.2.1. 몽고DB 연결
#### 29.2.2. ```MongoTemplate```
#### 29.2.3. Spring Data 몽고DB 레파지토리
### 29.3. Gemfire
### 29.4. Solr
#### 29.4.1. Solr 연결
#### 29.4.2. Spring Data Elasticsearch 레파지토리
### 29.5. Elasticsearch
#### 29.5.1. Elasticsearch 연결
#### 29.5.2. 스프링 데이터 Elasticsearch 레파지토리
## 30. 메시징
### 30.1. JMS
#### 30.1.1. HornetQ 지원
#### 30.1.2. ActiveMQ 지원
#### 30.1.3. JNDI ```ConnectionFactory``` 사용
#### 30.1.4. 메시지 전송
#### 30.1.5. 메시지 수신
## 31. 이메일 전송
## 32. JTA를 이용한 트랜잭션 분산
### 32.1. Atomikos 트랜잭션 매니저 사용
### 32.2. Bitronix 트랜잭션 매니저 사용
### 32.3. Java EE 에서 관리하는 트랜잭션 매니저 사용
### 32.4. XA 그리고 non-XA JMS 연결 혼합
### 32.5. 대안적인 내장형 트른잭션 매니저 지원
## 33. 스프링 통합
## 34. JMX를 통해서 모니터링과 관리
## [35. 테스팅](#테스팅)
### 35.1. 테스트 스코프 의존성
### 35.2. 스프링 애플리케이션 테스트
### 35.3. 스프링부트 애플리케이션 테스트
#### 35.3.1. 스팍Spock을 사용하여 스프링 부트 애플리케이션 테스트
### 35.4. 테스트 유틸리티
#### 35.4.1. ```ConfigFileApplicationContextInitializer```
#### 35.4.2. ```EnvironmentTestUtils```
#### 35.4.3. ```OutputCapture```
#### 35.4.4. ```TestRestTemplate```
## [36. 자동설정으로 개발하고 @Condition 사용하기](#자동설정으로 개발하고 @Condition 사용하기)
### 36.1. 자동설정 빈 이해
### 36.2. 자동설정 위치 후보지
### 36.3. 상황 애노테이션
#### 36.3.1. 클래스 상황
#### 36.3.2. 빈Bean 상황
#### 36.3.3. 리소스 상황
#### 36.3.4. 웹 애플리케이션 상황
#### 36.3.5. SpEL 표현식 상황
## 37. 웹소켓
## 38. 다음 읽을거리

# V. 스프링부트 액츄에터: 출시준비 기능들
## 39. 사용가능한 출시준비 기능들
## 40. [엔드포인트](#엔드포인트)
### 40.1. 엔드포인트 변경
### 40.2. 상태 정보 변경
### 40.3. 애플리케이션 정보 안내 변경
#### 40.3.1. 빌드 시간에 관한 속성 확장 자동화
#### 메이븐을 이용하여 속성 확장 자동화
#### 그레들을 이용하여 속성 확장 자동화
#### 40.3.2. 깃 커밋 정보
## 41. HTTP를 통해서 모니터링 및 관리
### 41.1. 세밀한 엔드포인트 노출
### 41.2. 관리 서버컨텍스트패스 변경
### 41.3. 관리 서버포트 변경
### 41.4. 관리 서버주소 변경
### 41.5. HTTP 엔드포인트 비활성화
### 41.6. 상태 엔드포인트에 대한 무기명 접근 제한
## 42. JMX를 통한 모니터링 및 관리
### 42.1. MBean 이름 변경
### 42.2. JMX 엔드포인트 비활성화
### 42.3. JMX용 Jolokia를 HTTP를 통해서 사용
#### 42.3.1. Jolokia 변경
#### 42.3.1. Jolokia 비활성화
## 43. 리모트쉘을 사용하여 모니터링 및 관리
### 43.1. 리모트쉘 연결
#### 43.1.1. 리모트쉘 자격credentials
### 43.2. 리모트쉘 확장
#### 43.2.1. 리모트쉘 명령어
#### 43.2.2. 리모트쉘 플러그인
## 44. 측정
### 44.1. 데이터소스 측정
### 44.2. 측정 기록
### 44.3. 공개 측정 추가
### 44.4. 측정 레파지토리
### 44.5. Coda Hale 측정
### 44.6. 메시지 채널 통합
## 45. 오디팅auditing
## 46. 추적Tracing
### 46.1. 추적 변경
## 47. 프로세스 모니터링
### 47.1. 설정 확장
### 47.2. 작성
## 48. 다음 읽을거리  

# VI. 클라우드 배포
## 49. Cloud Foundry
### 49.1. 서비스 연결
## 50. Heroku
## 51. CloudBees
## 52. Openshift
## 53. Google App Engine
## 54. 다음 읽을거리

# VII. [스프링부트 CLI](#스프링부트 CLI)
## 55. CLI 설치
## 56. CLI 사용
### 56.1. CLI를 이용해서 애플리케이션 실행
### 56.2. CLI에 의존성 추가
#### 56.2.1. "grab" 의존성 추정
#### 56.2.2. "grab" 협력 추정
#### "grab" 메타데이터 변경
#### 56.2.3. 기본 불러오기 문장
#### 56.2.4. 자동 main 메서드
### 56.3. 코드 테스트
### 56.4. 다양한 소스파일을 가진 애플리케이션
### 56.5. 애플리케이션 패키징
### 56.6. 새로운 프로젝트 준비
### 56.7. 내장형 쉘 사용
## 57. 그루비 빈즈 DSL을 통해서 애플리케이션 개발
## 58. 다음 읽을거리

# VIII. 빌드툴 플러그인
## 59. 스프링부트 메이븐 플러그인
### 59.1. 플러그인 추가
### 59.2. 실행가능한 jar 와 war 파일 패키징
## 60. 스프링부트 그레들 플러그인
### 60.1. 플러그인 추가
### 60.2. 버전 없이 의존성 정의
#### 60.2.1. 버전 관리 변경
### 60.3. 기본적인 배제 원칙
### 60.4. 실행가능한 jar 와 war 파일 패키징
### 60.5. 프로젝트 바로 실행
### 60.6. 스프링부트 플러그인 설정
### 60.7. 리패키징 설정
### 60.8. 맞춤 그레들 설정으로 리패키징
#### 60.8.1. 설정 사항
### 60.9. 그레들 플러그인의 동작방식 이해
### 60.10. 그레들을 이용해서 메이븐 레파지토리에 아티팩트 배포
#### 60.10.1. 그레들 설정을 이용한 상속적 의존성 관리 POM 제작
#### 60.10.2. 그레들 설정을 이용한 imports 의존성 관리 POM 제작
## 61. 다른 빌드 지원 시스템 지원
### 61.1. 리패키징 아카이브
### 61.2. 내포된 라이브러리
### 61.3. 메인 클래스 탐색
### 61.4. repackage 구현 예제
## 62. 다음 읽을 거리

# IX. '어떻게How-to' 가이드
## 63. 스프링부트 애플리케이션
### 63.1. 자동설정 문제해결
### 63.2. 시작 전 ```Environment``` 혹은 ```ApplicationContext``` 변경
### 63.3. ```ApplicationContext``` 계층 빌드(부모 혹은 루트 컨텍스트 추가)
### 63.4. non-web 애플리케이션 생성
## 64. 속성 및 설정
### 64.1. 스프링애플리케이션의 설정 확장
### 64.2. 애플리케이션의 외부 속성 위치 변경
### 64.3. '간략한' 커맨드라인 인자 사용
### 64.4. 외부 속성을 YAML로 정의
### 64.5. 활성 스프링 프로파일 설정
### 64.6. 환경 의존적 설정 변경
### [64.7. 외부 속성들의 빌트인 항목 살펴보기](#64.7. 외부 속성들의 빌트인 항목 살펴보기)
## 65. 내장형 서블릿 컨테이너
### 65.1. Servlet, Filter 혹은 ServletContextListener 를 애플리케이션에 추가
### 65.2. HTTP 포트 변경
### 65.3. HTTP 포트를 지정하지 않고 무작위로 사용
### 65.4. 실행시 HTTP Port 살펴보기
### 65.5. SSL 설정
### 65.6. 톰캣 설정
### 65.7. 톰캣의 다중커넥터 활성화
### 65.8. 톰캣을 프론트엔드 프록시 서버로 사용
### 65.9. 톰캣 대신 제티 사용
### 65.10. 제티 설정
### 65.11. 톰캣 대신 언더토우Undertow 사용
### 65.12. 언더토우 설정
### 65.13. 톰캣 7 사용
### 65.14. 제티 8 사용
### 65.15. ```@ServerEndpoint```를 사용해서 웹소켓 엔드포인트 생성
## 66. 스프링 MVC
### 66.1. JSON REST 서비스 작성
### 66.2. XML REST 서비스 작성
### 66.3. Jackson ObjectMapper 변경
### 66.4. ```@ResponseBody``` 렌더링 변경
### 66.5. ```Multipart``` 파일 업로드 제어
### 66.6. Spring MVC ```DispatcherServlet``` 끄기
### 66.7. 기본 MVC 설정 끄기
### 66.8. ViewResolver 변경
## 67. 로깅
### 67.1. 로깅을 위한 Logback 설정
### 67.2. 로깅을 위한 Log4j 설정
## 68. 데이터 접근
### 68.1. 데이터소스 설정
### 68.2. 복수 데이터소스 설정
### 68.3. 스프링 데이터 레파지토리 사용
### 68.4. 스프링 설정으로 부터 ```@Entity``` 정의 분리
### 68.5. JPA 속성 설정
### 68.6. ```EntityManagerFactory``` 변경
### 68.7. 복수 엔티티매니저 사용
### 68.8. 전통적인 ```persistence.xml```  사용
### 68.9. 스프링데이터 JPA와 몽고 레파지토리 사용
## [69. 데이터베이스 초기화](#69. 데이터베이스 초기화)
### 69.1. JPA 사용하여 데이터베이스 초기화
### 69.2. Hibernate를 사용하여 데이터베이스 초기화
### 69.3. Spring JDBC를 사용하여 데이터베이스 초기화
### 69.4. 스프링 배치 데이터베이스 초기화
### 69.5. 고차원 데이터베이스 마이그레이션 도구 사용
#### 69.5.1. 시작시 Flyway 실행하여 데이터베이스 마이그레이션
#### 69.5.2. 시작시 Liquibase를 실행하여 데이터베이스 마이그레이션
## 70. 배치 애플리케이션
### 70.1. 시작시 스프링 배치 작업 실행
## 71. 액츄에이터Actuator
### 71.1. 액츄에이터 엔드포인트의 주소 혹은 HTTP 포트 변경
### 71.2. 'whitelabel' 오류 페이지 변경
## 72. 시큐리티
### 72.1. 스프링부트 시큐리티 설정 끄기
### 72.2. ```AuthenticationManager```를 변경하고 사용자 계정 추가
## 73. 핫스와핑
### 73.1. 정적컨텐츠 다시 읽기
### 73.2. 컨테이너 재시작없이 타임리프Thymeleaf 템플렛 다시 읽기
### 73.3. 컨테이너 재시작없이 프리마크FreeMarker 템플렛 다시 읽기
### 73.4. 컨테이너 재시작없이 그루비Groovy 템플렛 다시 읽기
### 73.5. 컨테이너 재시작없이 벨로시티Velocity 템플렛 다시 읽기
### 73.6. 컨테이너 재시작없이 자바 클래스 다시 읽기
#### 73.6.1. 메이븐을 이용한 Spring Loaded 설정
#### 73.6.2. 그레들과 IntelliJ를 이용한 Spring Loaded 설정
## 74. 빌드
### 74.1. 메이븐으로 의존성 버전 변경
### 74.2. 메이븐으로 실행가능한 JAR 생성
### 74.3. 추가적인 실행가능한 JAR 생성
### 74.4. 실행가능한 jar 동작에 필요한 지정된 라이브러리 추출
### 74.5. 배제를 통한 실행할 수 없는 JAR 생성
### 74.6. 메이븐을 이용해서 스프링부트 애플리케이션 원격 디버그 시작
### 74.7. 그레들을 이용해서 스프링부트 애플리케이션 원격 디버그 시작
### 74.8. 앤트를 이용해서 실행가능한 아카이브 빌드
## 75. 전통적 배포
### 75.1. 배포가능한 war 파일 생성
### 75.2. 오래된 서블릿 컨테이너에 배포가능한 war 파일 생성
### 75.3. 기존의 애플리케이션을 스프링부트로 변환
### 75.4. 웹로직을 위한 war 배포
### 75.5. 오래된(Servlet 2.5) 컨테이너에 war 배포

# X. 부록
## A. 일반적인 애플리케이션 속성
## B. 메타데이터 설정
### B.1. 메타데이터 형식
#### B.1.1. 그룹 어트리뷰트
#### B.1.2. 속성 어트리뷰트
#### B.1.3. 반복적인 메타데이터 아이템
### B.2. 애노테이션 프로레서를 사용하여 메타데이터 생성
#### B.2.1. 내부 속성
#### B.2.2. 추가적인 메타데이터 추가
## C. 자동설정 클래스
### C.1. "spring-boot-autoconfigure" 모듈
### C.2. "spring-boot-actuator" 모듈
## D. 실행가능한 jar 형식
### D.1. 내부 JARs
#### D.1.1. 실행가능한 jar 파일 구조
#### D.1.2. 실행가능한 war 파일 구조
### D.2. 스프링부트의 "JarFile" 클래스
#### D.2.1. 표준 자바 "JarFile" 의 호환성
### D.3. 실행가능한 jars 실행
#### D.3.1. 매니페스트 실행
#### D.3.2. 아카이브 확장
### D.4. ```PropertiesLauncher``` 기능들
### D.5. 실행가능한 jar 제약사항
#### D.5.1. Zip 엔트리 압축
#### D.5.2. System ClassLoader
### D.6. 단독 jar 솔루션 대안

*****

# I. <a name="i-스프링부트-문서"></a>스프링부트 문서
이 섹션은 스프링부트 참고문서에 관해 간략하게 살펴본다. 문서의 나머지 부분들에 대한 지도라고 생각하자. 이 참고 가이드를 한줄한줄 열정적으로 읽을 수도 있고, 흥미가 없다면 지나쳐도 된다.

## 1. 문서에 대해
스프링부트 참고문서는 [html](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/reference/html), [pdf](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/reference/pdf/spring-boot-reference.pdf) 그리고 [epub](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/reference/epub/spring-boot-reference.epub) 문서로 제공된다. 최신판은 [http://docs.spring.io/spring-boot/docs/current/reference](http://docs.spring.io/spring-boot/docs/current/reference)에서 살펴볼 수 있다.

이 문서의 사본들은 자신이 사용하거나 다른 사람들에게 배포할 수 있으며, 인쇄 또는 전자출판시 사본에 저작권을 포함하고 어떤 수수료도 부과하지 않고 제공해야 한다.


## 2. 도움 구하기
스프링부트를 사용하면서 문제가 생겼다면, 우리가 도울 수 있다.

* [어떻게 하지?!](#'어떻게How-to' 가이드)를 이용 - 가장 일반적인 질문들에 대한 해결책을 제공한다.
* 스프링 기초를 배우기 - 스프링부트는 수많은 스프링 프로젝트를 빌드한다. [spring.io](http://spring.io) 웹사이트에서 제공하는 풍부한 참고문서들을 살펴본다. 만약 스프링을 이제 막 시작했다면, [guides](http://spring.io/guides)를 살펴보기 바란다.
* 궁금증을 묻는다 - 우리는 [http://stackoverflow.com/](http://stackoverflow.com/)에서 ```spring-boot```를 태깅한 질문들을 주시하고 있다.
* [https://github.com/spring-projects/spring-boot/issues](https://github.com/spring-projects/spring-boot/issues) 를 통해서 스프링부트와 관련된 버그를 보고한다.

> 스프링부트의 모든 것은 오픈소스이며, 문서가 함께 제공된다. 만약 문서에 문제가 있거나 개선해야할 사항이 있다면 [참여하라!](http://github.com/spring-projects/spring-boot/tree/master)

## 3. 첫걸음
만약, 스프링부트를 이제 막 시작했거나, '스프링'이 처음이라면, [여기서부터 시작하자.](#시작)
* 가볍게 살펴보기: [Overview](#스프링부트 소개) | [요구사항](#시스템 요구사항) | [설치](#스프링부트 설치)
* 튜토리얼: [1부](#초기 스프링부터 애플리케이션 개발) | [2부](#코드 작성)
* 예제 실행하기: [1부](#예제 실행) | [2부](#실행가능한 jar 생성)

## 4. 스프링부트 작동
정말 스프링부트를 시작할 준비가 되어있는가? [우리가 여러분을 도울 것이다.](#스프링부트 사용)
* **빌드 시스템**: [메이븐](#메이븐) | [그레들](#그레들) | [앤트](#앤트) | [스프링부트 스타터 POMs](#스프링부트 스타터)
* 좋은 연습거리: [코드 구성하기](#코드 구성하기) | [@Configuration](#설정@Congiruation 클래스들) | [@EnableAutoConfiguration](#자동설정(Auto-configuration)) | [Beans and Dependency Inject](#스프링 빈과 의존성 주입)
* 코드 실행: [IDE](#IDE에서 실행) | [패키징된 애플리케이션 실행](#패키징된 애플리케이션 실행) | [메이븐](#메이븐 플러그인 이용) | [그레들](#그레들 플러그인 이용)
* 애플리케이션 패키징: [출시를 위한 애플리케이션 패키징](#출시를 위한 애플리케이션 패키징)
* 스프링부트 CLI: [스프링부트 CLI](#스프링부트 CLI)

## 5. 스프링부트 기능 학습
스프링부트의 핵심기능에 관한 보다 상세한 내용이 필요한가? [그래서 준비했다!](#스프링부트 기능)
* 핵심기능: [SpringApplication](#스프링애플리케이션) | [외부설정](#외부설정) | [프로파일](#프로파일) | [로깅](#로깅)
* 웹 애플리케이션: [MVC](#Spring Web MVC framework) | [내장형 컨테이너](#내장형 서블릿 컨테이너 지원)
* 데이터 작업: [SQL](#SQL 데이터베이스 작업) | [NoSQL](#NoSQL 기술 작업)
* 메시징: [살펴보기](#메시징) | [JMS](#JMS)
* 테스팅: [살펴보기](#테스팅) | [부트애플리케이션](#스프링부트 애플리케이션) | [유틸들](#테스트 유틸리티)
* 확장: [자동설정](#자동설정으로 개발와 상황에 맞춰 사용) | [@Conditions](#컨디션 애노테이션 @Condition)

## 6. 출시
여러분이 스프링부트 애플리케이션을 출시하려는 시점에, 여러분이 좋아할만한 [몇가지 트릭들](#스프링부트 액츄에터: 출시준비 기능들)을 알려주겠다.

* 엔드포인트 관리: [Overview](#엔드포인트) | [변경](#엔드포인트 변경)
* 연결 항목: [HTTP](#HTTP를 통해서 모니터링 및 관리) | [JMX](#JMX를 통한 모니터링 및 관리) | [SSH](#리모트쉘을 사용하여 모니터링 및 관리)
* 모니터링: [측정](#감시auditing) | [감시](#추적Tracing)

## 7. 고급주제
마지막으로, 우리는 보다 고급진~ 사용자들을 위한 소재들을 제공한다.
* 클라우드 배포: [Cloud Foundry](#Cloud Foundry) | [Heroku](#Heroku) | [CloudBees](#CloudBees)
* 빌드툴 플러그인: [메이븐](#스프링부트 메이븐 플러그인) | [그레들](#60. 스프링부트 그레들 플러그인)
* 부록: [애플리케이션 속성](#애플리케이션 속성) | [자동설정 클래스](#자동설정 클래스) | [실행가능한 jar 형식](#D. 실행가능한 jar 형식)

# II. 시작<a name="시작"></a>
스프링부트 혹은 일반적인 '스프링'을 이제막 시작했다면, 여러분을 위한 섹션이다. 여기서 우리는 기본적인 '뭘?', '어떻게?' 와 '왜?'라는 질문들에 답을 한다. 여러분은 스프링부트 단독설치 설명과 함께 정중한 소개를 볼 수 있다. 우리는 먼저 스프링부트 애플리케이션을 빌드하고, 핵심 이론에 관하여 논의하며 진행하게 된다.

## 8. 스프링부트 소개<a name="스프링부트 소개"></a>
스프링부트는 스프링을 기반으로 하는, 바로 출시할 수 있는 수준의 '실행가능한', 단독실행형 애플리케이션을 만든다. 우리는 스프링플랫폼과 서드파티 라이브러리들에 대한 선택을 최소한의 논의로 결정할 수 있도록 했다. 스프링부트는 정말 최소한의 스프링 설정만 하면 된다.

여러분은 스프링부트를 통해서 ```java -jar```으로 시작할 수 있는 자바 애플리케이션 혹은 더 나아가 전통적인 war 배포물을 만들어낼 수 있다. 우리는 또한 커맨드라인에서 실행할 수 있는 'spring scripts'를 제공한다.

우리의 목표는 다음과 같다:
* 매우 빠르고 모든 스프링 개발에 관한 경험에 관한 광범위한 접근을 제공한다.
* 차이가 있기는 하겠지만, 기본값으로 부터 요구사항들에 따라 분기하며 빠르게 진행할 수 있다.
* 일반적으로 프로젝트에서 큰 영역을 차지하는 비기능적인 기능들을 제공한다(예를 들어, 내장형 서버, 시큐리티, 측정, 상태 점검, 외부 설정)
* 절대적으로 XML 설정을 요구하거나 더이상의 코드를 작성하지 않는다.

## 9. 시스템 요구사항<a name="시스템 요구사항"></a>
스프링부트 1.2.0.BUILD-SNAPSHOT은 JAVA 6 그리고 스프링 프레임워크 4.1.3. 혹은 그 이상을 요구한다. 명시인 빌드지원은 메이븐(3.2+) 그리고 그레들(1.12+)를 제공한다.
> Tip: Java 6에서는 스프링부트를 사용하는데 별 무리는 없지만, 우리는 가능하다면 Java 8을 사용하기를 권장한다.

### 9.1. 서블릿 컨테이너
다음 박스에 보이는 내장형 서블릿 컨테이너를 지원한다.
<table>
    <thead>
        <tr>
            <th>이름</th>
            <th>서블릿 버전</th>
            <th>자바 버전</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Tomcat 8</td>
            <td>3.1</td>
            <td>Java 7+</td>
        </tr>
        <tr>
            <td>Tomcat 7</td>
            <td>3.0</td>
            <td>Java 6+</td>
        </tr>
        <tr>
            <td>Jetty 9</td>
            <td>3.1</td>
            <td>Java 7+</td>
        </tr>
        <tr>
            <td>Jetty 8</td>
            <td>3.0</td>
            <td>Java 6+</td>
        </tr>
        <tr>
            <td>Undertow 1.1</td>
            <td>3.1</td>
            <td>Java 7+</td>
        </tr>
    </tbody>
</table>
또한 여러분은 서블릿 3.0+ 이상을 지원하는 컨테이너에 스프링부트 애플리케이션을 배포할 수 있다.

## 10. 스프링부트 설치<a name="스프링부트 설치"></a>
스프링 부트는 '클래식한' 자바 개발도구 혹은 커맨드라인 툴을 설치하여 사용할 수 있다. 그와는 상관없이 [Java SDK v1.6](http://www.java.com/) 혹은 그 이상을 필요로 한다. 시작하기에 앞서 현재 자바 설치버전을 확인하자.
```
$ java -version
```
만약 자바 개발이 처음이라면, 혹은 스프링부트를 실험해보고 싶다면 먼저 [스프링부트 CLI](#스프링부트 CLI)를 사용해보고, 그렇지 않다면 '클래식한' 설치 소개를 읽어보자.

> Tip: 스프링부트는 Java 1.6에서도 호환되지만, 가능하다면 최신버전의 자바를 사용하는 것을 고려하길 바란다.

### 10.1. 자바 개발자를 위한 설치법 소개
스프링부트는 표준 자바 라이브러리처럼 사용할 수 있다. ```spring-boot-*.jar``` 파일을 클래스패스에 적절하고 추가하면 된다. 스프링부트는 특별한 통합도구를 요구하지 않으며, 여러분은 다른 IDE 혹은 텍스트 에디터를 사용할 수 있다. 그리고 스프링부트 애플리케이션은 특별한 것이 없기 때문에, 여느 자바프로그램처럼 실행하고 디버그할 수 있다.

혹시 스프링부트 jars 를 복사해서 사용하려한다면, 우리는 의존성 관리를 지원하는 (메이븐 혹은 그레들 같은)빌드툴 사용을 권장한다.

#### 10.1.1. 메이븐 설치
스프링부트는 아파치 메이븐 3.0 혹은 그 이상의 버전에 호환된다. 만약 아직 메이븐을 설치하지 않았다면, [maven.apache.org](http://maven.apache.org/)에서 설명에 따라할 수 있을 것이다.

> 팁: 많은 운영체제들에서 메이븐은 패키지 매니저를 통해서 설치할 수 있다. 만약 OSX Homebrew 유저라면 ```brew install maven```으로, 우분투 유저라면 ``sudo apt-get install maven```으로 설치할 수 있다.

스프링부트 의존성은 ```org.springframework.boot groupid```를 한다. 일반적으로 Maven POM 파일은 ```spring-boot-starter-parent``` 프로젝트로부터 유전되었을 것이며 하나 혹은 그 이상의 [스프링부트 스타터 POMs](#스프링부트 스타터 POMs)에 관한 의존성을 정의했을 것이다. 스프링부트는 또한 실행가능한 jars 를 만들 수 있는 메이븐 플러그인을 선택할 수 있도록 한다.

여기 일반적인 pom.xml 파일이 있다:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>myproject</artifactId>
    <version>0.0.1-SNAPSHOT</version>

    <!-- Inherit defaults from Spring Boot -->
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>1.2.0.BUILD-SNAPSHOT</version>
    </parent>

    <!-- Add typical dependencies for a web application -->
    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
    </dependencies>

    <!-- Package as an executable jar -->
    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>

    <!-- Add Spring repositories -->
    <!-- (you don't need this if you are using a .RELEASE version) -->
    <repositories>
        <repository>
            <id>spring-snapshots</id>
            <url>http://repo.spring.io/snapshot</url>
            <snapshots><enabled>true</enabled></snapshots>
        </repository>
        <repository>
            <id>spring-milestones</id>
            <url>http://repo.spring.io/milestone</url>
        </repository>
    </repositories>
    <pluginRepositories>
        <pluginRepository>
            <id>spring-snapshots</id>
            <url>http://repo.spring.io/snapshot</url>
        </pluginRepository>
        <pluginRepository>
            <id>spring-milestones</id>
            <url>http://repo.spring.io/milestone</url>
        </pluginRepository>
    </pluginRepositories>
</project>
```

> 팁: ```spring-boot-starter-parent```는 스프링부트를 사용할 수 있는 좋은 방법이지만 모든 상황에 적합하지는 않다. 다른 부모 POM을 상속해야하는 경우가 있거나 기본 설정이 탐탁치 않을 수 있다. 그럴 때는 [13.1.2. 부모 POM 없이 스프링부트 사용](부모 POM 없이 스프링부트 사용)을 보고 ```import``` 스코프를 사용하여 적절한 해결책을 모색하기 바란다.

#### 10.1.2. 그레들 설치
스프링부트는 그레들 1.6 혹은 그 이상 버전에 호환된다. 만약 그레들이 설치되어 있지 않다면 <www.gradle.org>의 설명을 따라하면 된다.

스프링부트 의존성은 ```org.springframework.boot group```을 사용하여 정의된다. 일반적으로 여러분의 프로젝트는 하나 혹은 그 이상 [스프링부트 스타터 POMs](#스프링부트 스타터 POMs)에 관한 의존성을 정의했을 것이다. 스프링부트는 의존성을 간단하게 정의하고 실행가능한 jars를 생성하는데 매우 유용한 [그레들 플러그인](#60. 스프링부트 그레들 플러그인)을 제공한다.

##### 그레들 래퍼
그레들 래퍼는 프로젝트를 빌드하려는 떄에 그레들을 포함시킬 수 있는 좋은 방법이다. 그레들 래퍼는 빌드 과정에서 코드를 다루는 데 필요한 작은 스크립트와 라이브러리로 구성되어 있다. 이와 관련해서는 [www.gradle.org/docs/current/userguide/gradle_wrapper.html](www.gradle.org/docs/current/userguide/gradle_wrapper.html)을 통해 상세히 살펴볼 수 있다.

여기 일반적인 ```build.gradle```파일이 있다:
```gradle
buildscript {
    repositories {
        jcenter()
        maven { url "http://repo.spring.io/snapshot" }
        maven { url "http://repo.spring.io/milestone" }
    }
    dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:1.2.0.BUILD-SNAPSHOT")
    }
}

apply plugin: 'java'
apply plugin: 'spring-boot'

jar {
    baseName = 'myproject'
    version =  '0.0.1-SNAPSHOT'
}

repositories {
    jcenter()
    maven { url "http://repo.spring.io/snapshot" }
    maven { url "http://repo.spring.io/milestone" }
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    testCompile("org.springframework.boot:spring-boot-starter-test")
}
```

### 10.2. 스프링부트 CLI를 이용한 설치<a name="CLI를 이용한 설치"></a>
스프링부트 CLI는 스프링 프로토타입을 빠르게 만들려고할 때 쓸만한 커맨드라인 툴이다. [그루비](http://groovy.codehaus.org/) 스크립트를 실행할 수 있다으며, 이는 자바와 매우 유사한 문법을 가지고 있기에 별도로 다른 복잡한 코드를 작성할 필요가 없다.

스프링부트를 작업하데 CLI를 사용할 필요가 없을수도 있지만 스프링 애플리케이션을 만들 수 있는 가장 빠른 방법이라는 건 분명하다.

#### 10.2.1. 메뉴얼 설치법<a name="메뉴얼 설치법"></a>
스프링 CLI 배포판은 스프링 소프트웨어 저장소에서 내려받을 수 있다.

* [spring-boot-cli-1.2.0.BUILD-SNAPSHOT-bin.zip](http://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/1.2.0.BUILD-SNAPSHOT/spring-boot-cli-1.2.0.BUILD-SNAPSHOT-bin.zip)
* [spring-boot-cli-1.2.0.BUILD-SNAPSHOT-bin.tar.gz](http://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/1.2.0.BUILD-SNAPSHOT/spring-boot-cli-1.2.0.BUILD-SNAPSHOT-bin.tar.gz)

개발되고 있는 기능은 [스냅샷 배포판](http://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/) 을 통해 다운로드 가능하다.

다운받은 후, [INSTALL.txt](http://raw.github.com/spring-projects/spring-boot/master/spring-boot-cli/src/main/content/INSTALL.txt) 설명을 따라서 압축파일을 푼다. 정리하자면: ```.zip``` 파일 안에 ```bin/``` 디렉토리 안에 ```spring``` 스크립트(윈도우는 ```spring.bat``` 파일이 있다, 혹은 ```.jar```파일을 ```java -jar``` 를 이용할 수도 있다(스크립트는 클래스패스 오류를 줄이는 데 도움이 된다).
> 역자 주: 클래스패스나 환경설정 등의 이유로 스크립트 파일을 이용해서 실행하는 것을 권장한다.

#### 10.2.2. GVM을 이용한 설치법
GVM(그루비 환경 관리자)를 이용하면 다양한 버전의 그루비와 자바 바이너리 패키지를 관리할 수 있으며, 그 관리대상에는 그루비와 스프링부트 CLI까지 포함된다. [gvmtool.net](http://gvmtool.net/)에서 ```gvm```을 설치한 후 스프링부트를 설치하는 방법은,
```
$ gvm install springboot
$ spring --version
Spring Boot v1.2.0.BUILD-SNAPSHOT
```

혹시 CLI에서 개발중인 기능들을 사용하고 싶을 때도 쉽게 접근할 수 있다, 다음 추가설명을 따라서 해보자.
```
$ gvm install springboot dev /path/to/spring-boot/spring-boot-cli/target/spring-boot-cli-1.2.0.BUILD-SNAPSHOT-bin/spring-1.2.0.BUILD-SNAPSHOT/
$ gvm use springboot dev
$ spring --version
Spring CLI v1.2.0.BUILD-SNAPSHOT
```

이렇게 해서 로컬에 설치된 ```spring``` 인스턴스를 호출하면 GVM 저장소에 있는 ```dev``` 인스턴스가 대신 호출된다. 이렇게 해두면 스프링부트를 재빌드할때마다 대상 빌드 위치의 ```spring```은 최신상태를 유지한다.

설치가 완료된 후 다음과 같이:
```
$ gvm ls springboot

================================================================================
Available Springboot Versions
================================================================================
> + dev
* 1.2.0.BUILD-SNAPSHOT

================================================================================
+ - local version
* - installed
> - currently in use
================================================================================
```

```springboot```의 설치 상태를 확인할 수 있다.

#### 10.2.3. OSX Homebrew 설치법
만약에 맥과 [Homebrew](http://brew.sh/)를 사용하고 있다면, 스프링부트 CLI를 설치하는데 필요한 것은 다음과 같다:
```
$ brew tap pivotal/tap
$ brew install springboot
```

Homebrew는 ```/usr/local/bin```위치에 ```spring```을 설치한다.
> 노트: 만약 brew 설치버전이 보이지 않는다면 ```brew update```를 실행하여 다시한번 해보자.

#### 10.2.4. 커맨드라인 자동완성기능
스프링부트 CLI는 [Bash]()와 [zsh]()에서 사용가능한 커맨드 자동완성기능을 제공한다. 어느 쉘에서든지 ```source```스크립트(```sping```이라 불리는)를 사용하여, 개인이나 전체시스템 배쉬 자동완성기능을 사용할 수 있다. 데비안 시스템에서 사용가능한 전체시스템 스크립트는 ```/shell-completion/bash``` 그리고 새로운 쉘이 실행될 때 디렉토리의 모든 스크립트가 있다. 정석적으로 스크립트를 실행할 때는, GVM을 이용해서 설치한 경우라면:
```
$ . ~/.gvm/springboot/current/shell-completion/bash/spring
$ spring <HIT TAB HERE>
  grab  help  jar  run  test  version
```

> 노트: 만약 Homebrew를 이용하여 스프링부트 CLI를 설치했다면, 쉘에 자동으로 커맨드 자동완성 스크립트가 등록된다.

#### 10.2.5. 스프링 CLI로 빠르게 시작하는 예제
설치 여부를 확인할 수 있는 정말 간단한 웹 애플리케이션이 여기 있다. ```app.groovy```라는 이름으로 파일으 생성한다:
```groovy
@RestController
class ThisWillActuallyRun {

    @RequestMapping("/")
    String home() {
        "Hello World!"
    }

}
```

쉘에서 간단히 실행시킬 수 있다:
```
$ spring run app.groovy
```

> 노트: 애플리케이션을 처음 실행한다면 의존성 라이브러리들을 내려받는 시간이 걸릴 수 있다. 이후 실행은 매우 빠르게 처리될 것이다.

애용하는 브라우저를 이용해서 <localhost:8080> 접근하면 다음과 같은 내용을 확인할 수 있다:
```
Hello world!
```

### 10.3. 이전버전의 스프링부트로부터 업그레이드
이전에 출시한 스프링부트에서 업그레이드된 것들을 살펴보려면 [project wiki](http://github.com/spring-projects/spring-boot/wiki)에서 "출시노트"를 확인하라. 각 출시버전들에서 "신규 그리고 쓸만함" 항목에서 업그레이드에 관한 설명을 찾을 수 있을 것이다.

패키지 매니저 명령어를 이용하여(예를 들어 ```brew upgrade```) 설치된 CLI를 업그레이드하려거나 메뉴얼에 따라 CLI를 설치한 경우라면, [메뉴얼 설치법](#메뉴얼 설치법)을 상기하며 따라하여 오래된 참조링크를 제거하고 ```PATH```환경변수들을 갱신한다.

## 11. <a name="초기 스프링부터 애플리케이션 개발">초기 스프링부터 애플리케이션 개발</a>
이제 스프링부트의 핵심 기능 중 가장 강렬한 기능을 소개하는 간단한 "Hello world!" 웹 애플리케이션을 자바로 개발해보겠다. 대부분의 IDE들이 지원하는 메이븐을 이용하여 프로젝트를 빌드한다.

> 팁: <spring.io> 웹 사이트가 제공하는 많은 "Getting Started" 가이드들은 스프링부트를 사용하였다. 만약 특정한 문제가 발생하기 위한 방법을 찾고 있다면 먼저 다음의 항목들을 확인해보자.

시작하기에 앞서, 터미널을 열고 설치된 자바와 메이븐의 버전을 확인하자.
```
$ java -version
java version "1.7.0_51"
Java(TM) SE Runtime Environment (build 1.7.0_51-b13)
Java HotSpot(TM) 64-Bit Server VM (build 24.51-b03, mixed mode)
$ mvn -v
Apache Maven 3.1.1 (0728685237757ffbf44136acec0402957f723d9a; 2013-09-17 08:22:22-0700)
Maven home: /Users/user/tools/apache-maven-3.1.1
Java version: 1.7.0_51, vendor: Oracle Corporation
```

> 팁: 이 예제는 작업자 소유의 폴더를 생성해야한다. 이후 "현재 디렉토리"라고 하는 폴더는 생성가능한 폴더를 지칭한다.

### 11.1. POM 파일 생성
우리가 필요한 것은 시작하기 위해 ```pom.xml```을 생성하는 것이다. ```pom.xml```은 프로젝트를 빌드하는데 사용되는 레시피다. 애용하는 텍스트 에디터로 열고 다음 항목들을 추가해보자:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>myproject</artifactId>
    <version>0.0.1-SNAPSHOT</version>

    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>1.2.0.BUILD-SNAPSHOT</version>
    </parent>

    <!-- Additional lines to be added here... -->

    <!-- (you don't need this if you are using a .RELEASE version) -->
    <repositories>
        <repository>
            <id>spring-snapshots</id>
            <url>http://repo.spring.io/snapshot</url>
            <snapshots><enabled>true</enabled></snapshots>
        </repository>
        <repository>
            <id>spring-milestones</id>
            <url>http://repo.spring.io/milestone</url>
        </repository>
    </repositories>
    <pluginRepositories>
        <pluginRepository>
            <id>spring-snapshots</id>
            <url>http://repo.spring.io/snapshot</url>
        </pluginRepository>
        <pluginRepository>
            <id>spring-milestones</id>
            <url>http://repo.spring.io/milestone</url>
        </pluginRepository>
    </pluginRepositories>
</project>
```

이 레시피를 이용해서 빌드하고 나서, ```mvn package```를 실행하여 (```[WARNING] JAR will be empty - no content was marked for inclusion!```라는 메시지는 무시해도 된다).
> 노트: 여기서 중요한 점은 IDE(대부분의 메이븐을 이용한 빌드 기능을 제공하는 자바 IDE들)에서 프로젝트를 임포트하는 것이다. 간단하게 하기 위해, 우리는 텍스트 에디터 상에서 이 예제를 계속 진행할 것이다.

### 11.2. classpath 의존성 추가<a name="classpath 의존성 추가"></a>
스프링부트는 클래스패스classpath에 jar들을 추가하기 쉽도록 많은 "Starter POMs'를 제공한다. 샘플 애플리케이션은 POM의 ```parent``` 섹션에서 이미 ```spring-boot-starter-parent```을 사용하고 있다. ```spring-boot-starter-parent```는 유용한 기본 메이븐 기능들을 제공하는 특별한 스타터다. 또한 ```dependency-management``` 섹션에서는 의존성 에서 ```version``` 태그가 사라진 축복을 볼 수 있다.

다른 "Starter POMs"들은 애플리케이션의 특정 유형을 개발하는데 필요한 부분들에서 간소화된 의존성을 제공한다. 웹 애플리케션을 개발한다고 했을 때, 우리는 ```spring-boot-starter-web``` 의존성을 추가할 것이다. 그러나 그전에 현재 가지고 있는 것들을 살펴보자.
```
$ mvn dependency:tree

[INFO] com.example:myproject:jar:0.0.1-SNAPSHOT
```

```mvn dependency:tree``` 명령어는 현재 프로젝트의 의존성들을 표현한다. ```spring-boot-starter-parent``` 자신은 어떤 의존성도 가지지 않고 있는 것을 볼 수 있다. ```pom.xml```을 수정하여 ```spring-boot-starter-web``` 의존성을 ```parent``` 섹션 아래에 추가하자:

```xml
<dependencies>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>
</dependencies>
```

```mvn dependency:tree```을 다시 실행하면, 추가적인 의존성들이 많이 늘어난 것을 볼 수 있는데, 그 안에 톰캣웹서버와 스프링부트 자신이 포함되어 있다.

### 11.3. 코드 작성<a name="코드 작성"></a>

애플리케이션을 마무리 짓기 위해서 자바파일 하나를 생성해야한다. 메이븐은 기본적으로 ```src/main/java```에서 소스를 컴파일 하기때문에 우리는 이와 같은 폴더 구조를 만들어야 한다. 그런 후에 ```src/main/java/Example.java``` 파일을 생성한다.

```java
import org.springframework.boot.*;
import org.springframework.boot.autoconfigure.*;
import org.springframework.stereotype.*;
import org.springframework.web.bind.annotation.*;

@RestController
@EnableAutoConfiguration
public class Example {

    @RequestMapping("/")
    String home() {
        return "Hello World!";
    }

    public static void main(String[] args) throws Exception {
        SpringApplication.run(Example.class, args);
    }

}
```

더도말고 덜도말고 이정도의 코드면 충분하다. 이제 중요한 부분들을 진행하자.
#### 11.3.1. ```@RestController```와 ```@RequestMapping``` 애노테이션
```Example``` 클래스 사용된 첫번째 애노테이션은 ```@RestController``` 이다. 이것은 *stereotype* 애노테이션으로 알려져있다. 이것은 코드를 읽는 이들에게, 그리고 스프링에게 클래스가 수행하는 역할에 대한 힌트를 제공한다. 이 경우, 우리 클래스는 web ```@Controller```이며 스프링에서는 웹 리퀘스트를 처리하려할 때 고려대상이 된다.

```@RequestMapping``` 애노테이션은 "라우팅" 정보를 제공한다. 이것은 스프링에서 "/" 경로에 대한 HTTP 리퀘스트를 ```home``` 메서드에 연결한다. ```@RestController``` 애노테이션은 스프링에게 처리결과 문자열을 그대로 렌더링하여 호출자에게 반환하라고 이야기한다.

> 팁: ```@RestController```와 ```@RequestMapping``` 애노테이션들은 스프링 MVC 애노테이션(스프링부트에 정의된 것이 아니다). 스프링 레퍼런스 문서의 [MVC 섹션](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle#mvc) 에서 보다 상세한 내용을 볼 수 있다.

#### 11.3.2. ```@EnableAutoConfiguration``` 애노테이션
클래스에서 두번째로 사용된 애노테이션은 ```@EnableAutoConfiguration```이다. 이 애노테이션은 우리가 추가한 jar 의존성들을 바탕으로 하여 스프링을 설정하기를 바란다고 스프링부트가 "추측"하도록 한다. ```spring-boot-starter-web```를 추가하면 톰캣과 스프링MVC에 관해서 자동설정은 웹 애플리케이션을 개발할 것이고 그에 따라 스프링 설정을 할 것이라고 추측한다.

##### Starter POMs 와 자동설정Auto-Configuration

자동설정은 "Starter POMs"들에서 제대로 동작하도록 설계되었다. 그러나 두가지 개념이 사이를 비집을 수 없을 만큼 카이트하지는 않다. 자유롭게 "Starter POMs" 이외의 jar 파일에 대한 의존성을 추가할 수 있고 스프링부트는 여전히 애플리케이션의 관한 자동설정을 제공할 것이다.

#### 11.3.3. "main" 메서드
애플리케이션에서 마지막으로 살펴볼 부분은 ```main``` 메서드다. 이 메서드는 자바의 관례를 따르는 애플리케이션의 엔드포인트로써 표준 메서드다. 메인 메서드는 스프링부트의 ```SpringApplication``` 클래스의 ```run``` 메서드가 호출되는 메서드를 대표한다. ```SpringApplication```이 애플리케이션을 구동하면서 스프링은 톰캣웹서버에 대해 자동설정을 시작할 것이다. 우리는 ```SpringApplication```에게 ```Example.class```가 주요 스프링 컴포넌트라는 것을 말하기 위해서 ```run```메서드에 전달해야한다. ```args``` 배열은 커맨드라인 인자들을 탐색하여 전달한다.

### 11.4. 예제 실행<a name="예제 실행"></a>
이제 애플리케이션이 동작을 하고 있다. ```spring-boot-starter-parent``` POM에는 우리가 애플리케이션을 시작할 수 있는 ```run```이라고 하는 쓸만한 골Goal이 있다. 애플리케이션을 시작하기 위해 프로젝트의 루트디렉토리에서 ```mvn spring-boot:run```을 입력하자:
```
$ mvn spring-boot:run

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::  (v1.2.0.BUILD-SNAPSHOT)
....... . . .
....... . . . (log output here)
....... . . .
........ Started Example in 2.222 seconds (JVM running for 6.514)
```

브라우저를 실행하여 <localhost:8080>으로 이동하면 다음과 같은 출력결과를 볼 수 있다:
```
Hello World!
```

깔끔스럽게 애플리케이션을 종료하는 방법은 ```ctrl-c```를 치면 된다.

### 11.5. 실행가능한 jar 생성<a name="실행가능한 jar 생성"></a>
마지막으로 출시단계에서 실행할 수 있는 내장형 컨테이너를 이용해서 실행가능한 jar파일을 생성한다. 실행가능한 jars("묵직한fat jar"라고도 불리는) 은 코드가 실행되는데 필요한 의존성 jar들을 모두 포함하여 컴파일된 클래스들로 구성된 압축파일이다.

#### 실행가능한 jars와 자바

자바는 내장하고 있는 jar 파일들을 적재(jar 파일들은 jar를 포함한 파일일 뿐)하는 표준 방법을 제공하지 않는다. 이것은 배포가능한 자기실현 애플리케이션을 구상하는 이들에게는 걸림돌이 될 수밖에 없다.

이 문제를 해결하기 위해, 많은 개발자들은 jar를 'shaded'하는 방법을 사용한다. 'shaded` jar는 모든 jar파일로부터 모든 클래스파일들을 "uber jar"안에 한데묶어 버리는 것이다. shaded jar의 문제는 애플리케이션에서 실제로 사용하는 라이브러리들을 파악하기 어렵다는 것이다. 이는 많은 jar 파일들(물론 다른 내용이지만)에 존재하는 같은 이름의 파일명을 가지는 파일들이 문제가 될 수 있다.

스프링부트는 이를 [다르게 접근](#D. 실행가능한 jar 형식)하였고 실제로 내재하고 있는 jar파일들을 직접 접근가능하다.

실행가능한 jar을 생성하기 위해서는 ```spring-boot-maven-plugin```을 ```pom.xml```에 추가해야한다. 아래 코드를 ```dependencies``` 섹션 아래에 입력하자:
```xml
<build>
    <plugins>
        <plugin>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-maven-plugin</artifactId>
        </plugin>
    </plugins>
</build>
```

> 노트: ```spring-boot-starter-parent``` POM은 ```repackage```골과 연결된```<executions>``` 설정을 포함하고 있다. 만약 부모POM을 사용하지 않는다면 이 설정을 스스로 해야한다. 이와 관련된 내용은 [플러그인 문서](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/maven-plugin/usage.html)에 상세히 정리되어있다.

```pom.xml```파일을 저장하고 ```run package```를 커맨드라인에서 실행하자:
```
$ mvn package

[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building myproject 0.0.1-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] .... ..
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ myproject ---
[INFO] Building jar: /Users/developer/example/spring-boot-example/target/myproject-0.0.1-SNAPSHOT.jar
[INFO]
[INFO] --- spring-boot-maven-plugin:1.2.0.BUILD-SNAPSHOT:repackage (default) @ myproject ---
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
```

```target``` 디렉토리에 ```myproject-0.0.1-SNAPSHOT.jar```이 보인다면, 그 파일은 대략 10MB의 크기일 것이다. 혹시 안엘 살펴보고 싶다면 ```jar tvf```명령어를 사용할 수 있다:

```
$ jar tvf target/myproject-0.0.1-SNAPSHOT.jar
```

또한 ```target```디렉토리에 있는 작은 크기의 ```myproject-0.0.1-SNAPSHOT.jar.original``` 파일도 볼 수 있을 것이다. 이 파일은 스프링부트가 재포장repackage하기 전에 메이븐에서 생성한 원형jar다.

애플리케이션을 실행시키려면, ```java -jar```명령어를 사용한다:
```
$ java -jar target/myproject-0.0.1-SNAPSHOT.jar

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::  (v1.2.0.BUILD-SNAPSHOT)
....... . . .
....... . . . (log output here)
....... . . .
........ Started Example in 3.236 seconds (JVM running for 3.764)
```

앞에서 했듯이, 애플리케이션을 종료하려한다면 우아하게 ```ctrl-c```를 치면 된다.

## 12. 다음 읽을거리
이번 섹션에서는 스프링부트의 기본적인 내용과 애플리케이션을 작성하는 방법 등을 살펴보았다. 혹시나 여러분이 목표지향적인 개발자형이라면 [spring.io](http://spring.io)로 건너뛰어서 [바로 시작하기](http://spring.io/guides/) 가이드 중 하나를 체크아웃하고 "어떻게 스프링을 해결할 것인가?"하는 문제를 해결하고자 할 것이다: 그런 갈증을 해소시킬 수 있도록 스프링부트 ["어떻게 하지?how-to"](#'어떻게How-to' 가이드) 하고 참조할 수 있도록 해두었다.

혹은, 다음 과정인 [III. 스프링부트 사용](#스프링부트 사용)를 읽으면 된다. 정말 급하다면 [IV. 스프링부트 기능](#스프링부트 기능)로 건너뛰어가도 된다.


# III. 스프링부트 사용<a name="스프링부트 사용"></a>
이 섹션은 어떻게 스프링부트를 사용할지에 대해서 보다 세부적인 부분들을 살펴본다. 시스템 빌드, 자동설정 그리고 실행과 배포 옵션 등의 주제를 다룰 것이다. 또한 스프링부트에 관한 최선의 연습방법들도 다룬다. 비록 스프링부트의 특정한 부분들을 심도있게 다루지 않는다 해도 따르다보면 개발 프로세스가 조금은 쉬워질 것이다(특정 부분에 대해서 상세히 알려달라는 요청이 있지만 그건 극히 일부의 요청이며 그 요청은 누군가를 위한 참고가 될 가능성이 높다).

단순히 스프링부트를 실행시켜보는 것이 목적이라면, 이 섹션을 시작하기 전에 [바로 시작하기]()만 읽어도 충분할 것이다.

## 13. 빌드 시스템<a name="13. 빌드 시스템"></a>
선택한 빌드 시스템이 *의존성 관리* 지원은 필수적인 요구사항이며, 이를 위해서 "메이븐 중앙" 저장소repository에 배포된 아티팩트들을 사용할 수 있다. 스프링부트는 메이븐 혹은 그레들 중에서 하나를 선택해야 한다. 물론 스프링부트는 다른 빌드시스템(예를 들어 앤트Ant)에서 사용할 수 있지만, 특정 부분에 대해서는 정상동작하지 않을 수도 있다.

### 13.1. 메이븐<a name="메이븐"><a/>
메이븐 사용자는 ```spring-boot-starter-parent``` 프로젝트를 합리적인 기본값들을 상속하고 있다는 것을 살펴볼 수 있다. 부모 프로젝트는 다음과 같은 기능을 제공한다:

* 기본 컴파일러 레벨은 자바 1.6
* UTF8 소스 인코딩
* 의존성 관리 섹션에서, 공통 의존성들에서 ```<version>``` 태그와 관련한 부분은, ```spring-boot-dependencies``` POM을 상속
* 합리적인 [리소스 필터링](https://maven.apache.org/plugins/maven-resources-plugin/examples/filter.html)
* 합리적인 플러그인 설정([plugin exec](http://mojo.codehaus.org/exec-maven-plugin/), [surefire](http://maven.apache.org/surefire/maven-surefire-plugin/), [Git commit ID](https://github.com/ktoso/maven-git-commit-id-plugin), [shade](http://maven.apache.org/plugins/maven-shade-plugin/))
* application.properties 와 applicaton.yml을 위한 적절한 리소스 필터링

마지막으로, 기본설정파일들에서는 스프링 스타일의 플레이스홀더(```${...}```)와 유사한 형태로 메이븐 필터링을 이용해서 사용할 수 있는 ```@..@ 플레이스홀더를 제공한다(메이븐 속성 ```resource.delimiter```를 재정의할 수 있다).

#### 13.1.1. 스프링부트 스타터 부모 상속
```spring-boot-starter-parent```를 ```parent```에 정의하면 스프링부트와 관련된 기본적인 설정을 프로젝트에 상속한다.
```xml
<!-- Inherit defaults from Spring Boot -->
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>1.2.0.BUILD-SNAPSHOT</version>
</parent>
```
> 노트: 이 의존성에 대해서만은 스프링부트 버전넘버가 필요하다. starters를 추가하는 경에는 버전넘버를 생략해도 된다. -> spring-boot-starter-parent에는 starter 들의 버전이 기본설정되어 있다. 필요에 따라서는 자신이 필요한 버전```<version><version>```을 정의하여 사용할 수 있다. 다만, 자동설정에서 문제가 발생할 수도 있다.

#### 13.1.2. 부모 POM 없이 스프링부트 사용<a name="부모 POM 없이 스프링부트 사용"></a>
모든 이들이 ```spring-boot-starter-parent```을 상속하는 것을 좋아하지는 않는다. 별도로 사용하는 기본 부모가 있거나 필요하다면, 메이븐 설정에서 명시적으로 선언하는 것을 선호하기도 할 것이다.

```spring-boot-starter-parent``` 사용을 원하지 않으면서도, 의존성 관리의 이점(플러그인 관리는 제외)은 유지하길 바란다면 ```scope=import``` 의존성을 사용할 수 있다:
```xml
<dependencyManagement>
     <dependencies>
        <dependency>
            <!-- Import dependency management from Spring Boot -->
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-dependencies</artifactId>
            <version>1.2.0.BUILD-SNAPSHOT</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```

#### 13.1.3. 자바 버전 변경
```spring-boot-starter-parent```는 보수적으로 자바 안정성을 고려했다. 필요에 따라 최신 자바 버전을 사용하려한다면 ```java.version``` 프로퍼티를 추가하면 된다:
```xml
<properties>
    <java.version>1.8</java.version>
</properties>
```

#### 13.1.4. 스프링부트 메이븐 플러그인 사용
스프링부트는 실행가능한 jar로 프로젝트를 압축하기 위해 메이븐 플러그인을 포함하고 있다. 이 플러그인을 추가하고 싶다면 ```<plugin>``` 섹션에 다음과 같이 추가한다:
```xml
<build>
    <plugins>
        <plugin>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-maven-plugin</artifactId>
        </plugin>
    </plugins>
</build>
```
> 노트: 스프링부트 스타터 부모 POM을 사용하고 있는 상황에서, 플러그인 추가가 필요할 때, 부모에 정의되어 있는 설정을 변경하려하지 않는한 추가적인 설정을 할 필요는 없다. -> 플러그인 설정도 스타터 부모 POM에 설정이 되어 있으니 따로 추가하지 않아도 된다.

### 13.2. 그레들<a name="그레들"></a>
그레들 사용자는 ```dependencies``` 섹션에 "starter POM"들을 바로 추가할 수 있다. 메이븐과는 달리 설정에서 "최상이 부모super parent"를 설정에 추가할 필요가 없다.
```
apply plugin: 'java'

repositories { jcenter() }
dependencies {
    compile("org.springframework.boot:spring-boot-starter-web:1.2.0.BUILD-SNAPSHOT")
}
```

또한 [spring-boot-gradle-plugin](#60. 스프링부트 그레들 플러그인)은 실행가능한 jar를 생성하는 태스크들을 제공하고 소스를 바탕으로 프로젝트를 실행하는 것이 가능하다. 거기다가 ```ResolutionStrategy```을 추가하여 [의존성의 버전넘버를 생략하는 것](#버전 없이 의존성 정의)도 가능하다:
```
buildscript {
    repositories { jcenter() }
    dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:1.2.0.BUILD-SNAPSHOT")
    }
}

apply plugin: 'java'
apply plugin: 'spring-boot'

repositories { jcenter() }
dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    testCompile("org.springframework.boot:spring-boot-starter-test")
}
```

### 13.3. 앤트<a name="앤트"></a>
스프링부트 프로젝트는 아파치 앤트를 이용해서도 빌드가 가능하다. 그러나 특별한 지원이나 플러그인을 제공하지는 않는다. 앤트 스크립트는 아이피Ivy 의존성 관리 시스템을 사용하여 starter POM들을 추가한다.

(74.8 앤트를 이용해서 실행가능한 아카이브 빌드)[#앤트를 이용해서 실행가능한 아카이브 빌드]을 보면 "어떻게 하지?"에 관한 보다 상세한 안내를 받을 수 있다.

### 13.4. 스프링부트 스타터 POM 목록<a name="스프링부트 스타터 POMs"></a>
스타터 POM들은 애플리케이션에 포함된 의존성 명세의 편의성을 제공한다. 필요하다면, 스프링과 관련 기술에 관한 모든 것을, 예제 코드를 찾아보고 의존성 명세 복사해서 붙이지 않아도 되는, 한곳에 해결할 수 있는 대형만물상을 가지게 된 것이다. 예를 들어, 스프링과 데이터처리용 JPA를 바탕으로 시작하려 한다면, 프로젝트 의존성에 ```spring-boot-starter-data-jpa``` 만 추가하면,바로 시작할 수 있다.

스타터들은 프로젝트에서 필요로하고 빠르게 실행하고 일관성있고 상황에 따라 관리할 수 의존성들을 바탕으로 구성되어 있다.

#### 이름이 가진 의미
모든 스타터들은 ```spring-boot-starter-*,``` 라고 하는 작명규칙을 따른다. ```*```은 애플리케이션의 특별한 유형을 정의한다. 이 이름구조는 필요한 스타터를 찾을때 유용하다. 많은 IDE의 메이븐 통합시스템은 이름을 통해서 의존성들을 검색한다. 예를 들어, STS 플러그인이 설치된 이클립스에서, POM에디터에서 ```ctrl-space```를 치고 ```"spring-boot-starter"```라고 입력하면 관련한 목록이 보인다.

다음 목록은 ```org.springframework.boot``` 그룹 하위의 스프링부트에서 제공하는 애플리케이션 스타터들이다:

#### 표 13.1. 스프링부트 애플리케이션 스타터들
|Name|Description|
|----|-----------|
|```spring-boot-starter```|The core Spring Boot starter, including auto-configuration support, logging and YAML.|
|```spring-boot-starter-actuator```|Production ready features to help you monitor and manage your application.|
|```spring-boot-starter-amqp```|Support for the “Advanced Message Queuing Protocol” via spring-rabbit.|
|```spring-boot-starter-aop```|Support for aspect-oriented programming including spring-aop and AspectJ.|
|```spring-boot-starter-batch```|Support for “Spring Batch” including HSQLDB database.|
|```spring-boot-starter-data-elasticsearch```|Support for the Elasticsearch search and analytics engine including spring-data-elasticsearch.|
|```spring-boot-starter-data-gemfire```|Support for the GemFire distributed data store including spring-data-gemfire.|
|```spring-boot-starter-data-jpa```|Support for the “Java Persistence API” including spring-data-jpa, spring-orm and Hibernate.|
|```spring-boot-starter-data-mongodb```|Support for the MongoDB NoSQL Database, including spring-data-mongodb.|
|```spring-boot-starter-data-rest```|Support for exposing Spring Data repositories over REST via spring-data-rest-webmvc.|
|```spring-boot-starter-data-solr```|Support for the Apache Solr search platform, including spring-data-solr.|
|```spring-boot-starter-freemarker```|Support for the FreeMarker templating engine|
|```spring-boot-starter-groovy-templates```|Support for the Groovy templating engine|
|```spring-boot-starter-hornetq```|Support for “Java Message Service API” via HornetQ.|
|```spring-boot-starter-integration```|Support for common spring-integration modules.|
|```spring-boot-starter-jdbc```|Support for JDBC databases.|
|```spring-boot-starter-jta-atomikos```|Support for JTA distributed transactions via Atomikos.|
|```spring-boot-starter-jta-bitronix```|Support for JTA distributed transactions via Bitronix.|
|```spring-boot-starter-mobile```|Support for spring-mobile|
|```spring-boot-starter-redis```|Support for the REDIS key-value data store, including spring-redis.|
|```spring-boot-starter-remote-shell```|Support for CRaSH.|
|```spring-boot-starter-security```|Support for spring-security.|
|```spring-boot-starter-social-facebook```|Support for spring-social-facebook.|
|```spring-boot-starter-social-linkedin```|Support for spring-social-linkedin.|
|```spring-boot-starter-social-twitter```|Support for spring-social-twitter.|
|```spring-boot-starter-test```|Support for common test dependencies, including JUnit, Hamcrest and Mockito along with the spring-test module.|
|```spring-boot-starter-thymeleaf```|Support for the Thymeleaf templating engine, including integration with Spring.|
|```spring-boot-starter-velocity```|Support for the Velocity templating engine|
|```spring-boot-starter-web```|Support for full-stack web development, including Tomcat and spring-webmvc.|
|```spring-boot-starter-websocket```|Support for WebSocket development.|
|```spring-boot-starter-ws```|Support for Spring Web Services|

애플리케이션 스타터에 추가적으로, 다음의 스타터들을 추가하면 [출시준비](#스프링부트 액츄에터: 출시준비 기능들) 기능을 사용할 수 있게 된다.

#### 테이블 13.2. 스프링부트 출시준비 스타터
|Name|Description|
|----|-----------|
|```spring-boot-starter-actuator```|Adds production ready features such as metrics and monitoring.|
|```spring-boot-starter-remote-shell```|Adds remote ssh shell support.|

마지막으로, 스프링부트는 원하는 특정한 기술 페이셋Facet으로 변경하거나 제외하고자 할 때 사용할 수 있는 몇몇 스타터들을 포함하고 있다.

#### 테이블 13.3. 스프링부트 기술 스타터
|Name|Description|
|----|-----------|
|```spring-boot-starter-jetty```|Imports the Jetty HTTP engine (to be used as an alternative to Tomcat)|
|```spring-boot-starter-log4j```|Support the Log4J logging framework|
|```spring-boot-starter-logging```|Import Spring Boot’s default logging framework (Logback).|
|```spring-boot-starter-tomcat```|Import Spring Boot’s default HTTP engine (Tomcat).|
|```spring-boot-starter-undertow```|Imports the Undertow HTTP engine (to be used as an alternative to Tomcat)|

> 팁: 깃헙에 있는 ```spring-boot-starter``` 모듈에서 [README 파일](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-starters/README.adoc)을 살펴보면, 추가적으로 커뮤니티에서 제공하는 스타터 POM들을 볼 수 있다.

## 14. 코드 구성하기<a name="코드 구성하기"></a>
스프링부트는 동작하는 데 별다른 코드 레이아웃을 요구하지는 않지만, 도움이 되는 몇가지 연습할 수 있는 것들이 있다.

### 14.1. 'default' 패키지 이용
"기본 패키지default package"에 있는 것으로 간주되는 패키지 선언을 포함하지 않는 클래스를 위치해 있는 경우, "기본 패키지"의 사용은 권장되지 않는 피해야하는 사항이다. ```@ComponentScan``` 혹은 ```@EntityScan``` 애노테이션을 사용하는 스프링부트 애플리케이션에 포함되어 있는 모든 jar들의 클래스를 읽는 과정에서 문제가 발생할 수 있다.

> 팁: 우리는 자바가 권장하는 패키지 작명관례와 도메인명을 역순으로 사용하는 것을 권장한다.

### 14.2. 메인 애플리케이션 클래스 위치
일반적으로 메인 애플리케이션 클래스는 다른 클래스들보다 최상위 패키지에 위치하는 것을 권장한다. ```@EnableAutoConfiguration``` 애노테이션은 메인 클래스에 선언되는 경우가 일반적인데, 이는 명시적인 아이템들을 대상으로 하는 기본 "검색 패키지"를 선언하는 것이기도 하다. 예를 들어, 애플리케이션에서 JPA를 사용하고 있다면, ```@EnableAutoConfiguration``` 애노테이션 선언된 클래스의 패키지는 ```@Entity``` 항목들을 검색하여 사용할 것이다.

```@ComponentScan``` 애노테이션을 루트 패키지에서 사용하면 ```basePackage``` 속성을 선언없이 사용가능하다.

여기 기본적인 계층이 있다:
```
com
 +- example
     +- myproject
         +- Application.java
         |
         +- domain
         |   +- Customer.java
         |   +- CustomerRepository.java
         |
         +- service
         |   +- CustomerService.java
         |
         +- web
             +- CustomerController.java
```

```Application.java``` 파일에는 ```main```메서드와 ```@Configuration```가 선언되어 있다.  

```java
package com.example.myproject;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@EnableAutoConfiguration
@ComponentScan
public class Application {

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}

```

## 15. 설정@Congiruation 클래스들<a name="설정@Congiruation 클래스들"></a>
**스프링부트는 자바 기반의 설정을 선호한다.** 또한 XML과 함께 사용하더라도  ```@Configuration```이 선언되어 있는 클래스에서 ```SpringApplication.run()```을 호출하는 것이 가능하다. 항상 클래스에 ```main```메서드를 정의해두면 주요 ```@Configuration```의 좋은 후보군이 된다.

> 팁: 많은 스프링설정 예제들이 XML 설정을 사용하여 배포된다. 가능하다면 동등한 자바 기반의 설정으로 사용하자. ```enable*``` 애노테이션으로 검색을 하면 좋은 시작점이 될 것이다.

### 15.1. 추가된 설정 클래스들 불러오기
모든 설정을 ```@Configuration```이 선언되어 있는 단일 클래스에 몰아 넣을 필요는 없다. ```@Import``` 애노테이션을 통해서 추가적으로 설정클래스를 사용할 수 있다. 혹은, ```@ComponentScan```을 사용하여 ```@Configuration``` 클래스들을 포함한 모든 스프링 컴포넌트를 자동으로 등록가능하다.

### 15.2. XML 설정 불러오기
혹시라도 무조건 XML 기반의 설정을 사용해야겠다 하더라도, 우리는 ```@Configuration``` 클래스에서 시작하기를 권장한다. ```@ImportResource``` 애노테이션을 사용하여 XML 설정 파일을 읽어들여서 사용가능하다.

## 16. 자동설정(Auto-configuration)<a name="자동설정(Auto-configuration)"></a>
스프링부트 자동설정은 사용자가 추가한 jar 의존성을 기반으로 하여 스프링 애플리케이션을 자동으로 설정하려 한다. 예를 들어, 클래스패스상에 ```HSQLDB```가 있다면 데이터베이스 커넥션 빈들을 수동으로 설정하지 않아도, 이미 인-메모리 데이터베이스에 대해서 자동으로 설정되어 있을 것이다.

자동설정을 하도록 선택하려면 ```@Configuration``` 클래스에 ```@EnableAutoConfiguration``` 애노테이션을 추가하면 된다.

> 팁: 지금까지 ```@EnableAutoConfiguration``` 애노테이션만 추가해본 적이 없다면, 기본 ```@Configuration``` 클래스에 해당 애노테이션을 추가하기를 권장한다.

### 16.1. 점진적으로 자동설정을 대체
자동설정은 확장성이 없다, 특정 시점이 되면 자동설정의 특정 부분들을 대체하는 설정을 정의해야 한다. 예를 들어, ```DataSource```빈을 추가하고자 할 때, 기본 내장형 데이터베이스의 지원은 걷어내야 한다.

현재 어떤 자동설정이 적용되었는지, 왜 사용되었는지를 찾아보고자 한다면 애플리케이션을 실행하면서 ```-debug``` 스위치를 함께 실행하면 된다. 이렇게 하면 콘솔을 통해 자동설정 보고서가 출력된다.
```
./gradlew bootrun -debug
```

### 16.2. 특정한 자동설정 비활성화
사용할 필요가 없는 특정 자동설정 클래스들을 찾았다면, ```@EnableAutoConfiguration``` 의 제외속성exclude attribute을 사용하여 그것들을 비활성화 할 수 있다.
```java
import org.springframework.boot.autoconfigure.*;
import org.springframework.boot.autoconfigure.jdbc.*;
import org.springframework.context.annotation.*;

@Configuration
@EnableAutoConfiguration(exclude={DataSourceAutoConfiguration.class})
public class MyConfiguration {
}
```

## 17. 스프링 빈과 의존성 주입<a name="스프링 빈과 의존성 주입"></a>
자유롭게 표준 스프링 프레임워크 기술을 사용하여 자유롭게 빈을 정의하고 그것들의 의존성을 주입받을 것이다. 간단히 정리하면, 우리는 ```@ComponentScan```을 사용하여 빈을 검색하고 이와 연계하여 ```@Autowired``` 생성자 주입 등을 활용하고 있다.

위에서 제안한 대로 코드를 구성(최상위 패키지에 애플리케이션 클래스 위치)했다면, ```@ComponentScan```에 인자를 추가하지 않고 사용할 수 있다. 모든 애플리케이션 컴포넌트들(```@Component```, ```@Service```, ```@Repository```, ```@Controller``` 등)이 스프링 빈으로 자동 등록될 것이다.

다음에서 예로 들고 있는 ```@Service``` 빈은 생성자 주입을 이용해서 ```RiskAssessor``` 빈을 제공받고 있다.
```java
package com.example.service;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

@Service
public class DatabaseAccountService implements AccountService {

    private final RiskAssessor riskAssessor;

    @Autowired
    public DatabaseAccountService(RiskAssessor riskAssessor) {
        this.riskAssessor = riskAssessor;
    }

    // ...

}
```

> 팁: 생성자 주입이 어떻게 사용되는지 따라가다보면 ```riskAssessor``` 필드에 ```final```이 선언되어 있는데, 이후에는 변경되지 않을 것이라는 표시다.

## 18. ```@SpringBootApplication```애노테이션 사용
많은 스프링부트 개발자들이 그들의 메인 클래스에 ```@Configuration```, ```@EnableAutoConfiguration``` 과 ```@ComponentScan``` 애노테이션을 선언하고 있다. 이 애노테이션들은 함께 쓰이는 것이 잦은 편이기에(위에서 [좋은 연습예제](#코드 구성하기)를 따라서 해봤다면), 스프링부트에서 제공하는 ```@SpringBootApplication``` 으로 대체할 수도 있다.

```@SpringBootApplication``` 애노테이션은 ```@Configuration```, ```@EnableAutoConfiguration``` 과 ```@ComponentScan```의 기본속성을 사용한 것과 동일하다:
```java
package com.example.myproject;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication // same as @Configuration @EnableAutoConfiguration @ComponentScan
public class Application {

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}
```

## 19. 애플리케이션 실행
jar로 압축하고 내장된 HTTP 서버를 사용하면서 얻게되는 가장 큰 이득은 다른 것들과는 상관없이 독립적으로 실행할 수 있다는 것이다. 스프링부트 애플리케이션을 디버깅하는 것은 쉽다. 별도의 IDE 플러그인이나 확장이 필요하지 않다.

> 노트: 이 섹션은 jar로 압축된 경우에 한정적이지만, 애플리케이션을 war 패키지로 압축한다면 사용하는 서버나 IDE 문서를 참조해야 한다.

### 19.1. IDE에서 실행<a name="IDE에서 실행"></a>
스프링부트 애플리케이션은 IDE에서 간단한 자바 애플리케이션처럼 실행할 수 있다. 그러나, 처음에는 프로젝트를 불러와야 한다. 불러오는 과정은 IDE와 빌드 시스템에 따라 다양하다. 대부분의 IDE는 메이븐 프로젝트로 바로 불러올 수 있다, 이클립스 사용자를 예로 들면 파일 메뉴에서 ```import -> Existing Maven Project```로 선택할 수 있다.

혹시나 IDE에서 프로젝트를 바로 불러올 수 없다면, 빌드 플러그인을 사용하여 IDE 메타태그를 생성할 수 있다. 메이븐에는 [이클립스](http://maven.apache.org/plugins/maven-eclipse-plugin/)와 [IDEA](http://maven.apache.org/plugins/maven-idea-plugin/)를 포함하고 있다; 그레들은 보다 [다양한 IDE들](http://www.gradle.org/docs/current/userguide/ide_support.html)을 지원한다.

> 팁: 웹 애플리케이션을 실행하다 보면 종종 "Port already in use" 라는 에러를 접하게 될 것이다. STS 사용자는 ```Run`` 보다 ```Relaunch``` 버튼을 사용하여 이미 존재하는 인스턴스를 종료하도록 할 수 있다.

### 19.2. 패키징된 애플리케이션 실행<a name="패키징된 애플리케이션 실행"></a>
만약 스프링부트 메이븐과 그레들 플러그인을 사용하여 생성한 실행가능한 jar는 ```java -jar```를 사용하여 애플리케이션을 실행할 수 있다. 예를 들어:

```
$ java -jar target/myproject-0.0.1-SNAPSHOT.jar
```

또한 압축된 애플리케이션은 원격 디버깅 지원이 가능하도록 설정하여 실행하는 것도 가능하다. 다음과 같이 패키지 애플리케이션에 디버거를 추가할 수 있다:

```
$ java -Xdebug -Xrunjdwp:server=y,transport=dt_socket,address=8000,suspend=n \
       -jar target/myproject-0.0.1-SNAPSHOT.jar
```

### 19.3. 메이븐 플러그인 이용<a name="메이븐 플러그인 이용"></a>
스프링부트 메이븐 플러그인에 포함되어 있는 ```run``` 골은 빠르게 컴파일하고 애플리케이션을 실행할 수 있다. 애플리케이션은 분해도에서 실행되며 인스턴스 "핫" 리로드를 위해서 리소스를 수정할 수 있다.

```
$ mvn spring-boot:run
```

유용한 운영체제 환경 변수:

```
$ export MAVEN_OPTS=-Xmx1024m -XX:MaxPermSize=128M -Djava.security.egd=file:/dev/./urandom
```
("egd" 설정은 톰캣이 구동되는 과정에서 세션키를 위한 엔트로피 자원을 재빨리 제공하여 구동속도를 향상시킨다.)

### 19.4. 그레들 플러그인 이용<a name="그레들 플러그인 이용"></a>
스프링부트 그레들 플러그인 또한 애플리케이션을 실행할 때 ```run``` 골을 분해도처럼 사용한다.

```
$ gradle bootRun
```

유용한 운영체제 환경변수:
```
$ export JAVA_OPTS=-Xmx1024m -XX:MaxPermSize=128M -Djava.security.egd=file:/dev/./urandom
```

### 19.5. 핫스와핑
스프링부트 애플리케이션은 순수한 자바 애플리케이션이며, JVM 핫스와핑hot-swapping 은
바깥의 영역에서 진행된다. JVM 핫스와핑은 어느정도 대체가능한 바이트코드로 제한되며, 보다 나은 해결책으로 [Spring loaded](https://github.com/spring-projects/spring-loaded) 프로젝트 혹은 [JRebel](http://zeroturnaround.com/software/jrebel/)을 사용할 수 있다.

보다 세부적인 내용에 대해서는  [핫스와핑 "어떻게 하지"](#핫스와핑)를 살펴보자.

## 20. 출시를 위한 애플리케이션 패키징<a name="출시를 위한 애플리케이션 패키징"></a>
실행가능한 jar는 출시 배포를 위해서도 사용가능하다. 그 자체로 실행가능하며, 또한 클라우드 기반의 배포에도 적합하다.

추가적으로 "출시 준비" 기능으로, 상태, 감시 그리고 엔드포인트인 REST 혹은 JMX에 대한 측정이 가능하니. ```spring-boot-actuator```를 추가하는 것을 고려해보라.보다 자세한 내용은 [5부. "스프링부트 액츄에터: 출시준비 기능들"](#스프링부트 액츄에터: 출시준비 기능들)을 읽어보기 바란다.

## 21. 다음 읽을거리
좋은 예제를 따라서 연습하면서 스프링부트를 어떻게 사용해야하는지를 이해하는데 충분했을 것이라 생각한다. 이제는 [스프링부트 기능](#스프링부트 기능)에서 보다 깊이있게 배워볼 것이나 이를 넘기고 스프링부트의 "[출시준비](#스프링부트 액츄에터: 출시준비 기능들)" 측면을 읽어도 된다.

# IV. 스프링부트 기능<a name="스프링부트 기능"></a>
이 섹션은 스프링부트의 상세한 부분으로 뛰어든다. 여기서 사용하려 하고 변경하려고 하는 핵심 기능들에 관하여 배우게 된다. 혹시나 준비되지 않았다면, [II. "시작"](#시작) 그리고 [III. "스프링부트 사용"](#스프링부트 사용) 섹션을 읽어두면 기본적인 배경지식을 갖출 수 있을 것이다.

## 22. 스프링애플리케이션<a name="스프링애플리케이션"></a>
```SpringApplication``` 클래스는 ```main()```메서드로부터 시작된 스프링 애플리케이션이 구동을 위한 관례적인 경로를 제공한다. 많은 상황에서 ```SpringApplication.run``` 정적 메서드를 정의하고 있을 것이다.

```java
public static void main(String[] args) {
    SpringApplication.run(MySpringConfiguration.class, args);
}
```

애플리케이션이 시작할 때 다음과 유사한 형태로 실행될 것이다:
```
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::   v1.2.0.BUILD-SNAPSHOT

2013-07-31 00:08:16.117  INFO 56603 --- [           main] o.s.b.s.app.SampleApplication            : Starting SampleApplication v0.1.0 on mycomputer with PID 56603 (/apps/myapp.jar started by pwebb)
2013-07-31 00:08:16.166  INFO 56603 --- [           main] ationConfigEmbeddedWebApplicationContext : Refreshing org.springframework.boot.context.embedded.AnnotationConfigEmbeddedWebApplicationContext@6e5a8246: startup date [Wed Jul 31 00:08:16 PDT 2013]; root of context hierarchy
2014-03-04 13:09:54.912  INFO 41370 --- [           main] .t.TomcatEmbeddedServletContainerFactory : Server initialized with port: 8080
2014-03-04 13:09:56.501  INFO 41370 --- [           main] o.s.b.s.app.SampleApplication            : Started SampleApplication in 2.992 seconds (JVM running for 3.658)
```

기본적으로 ```INFO``` 로깅 메시지에서는, 사용자가 실행한 애플리케이션의 구동과 관련된 세부항목들을 보여준다.

### 22.1. 배너 수정
구동시 보여주는 배너를 변경하려면 클래스패스 상에 ```banner.txt```를 추가하거나 ```banner.location```에서 파일의 경로를 설정할 수 있다. 일반적이지 않은 인코딩을 사용하는 경우에는 ```banner.encoding```(기본 UTF-8)으로 설정할 수 있다.

### 22.2. 스프링애플리케이션 수정
기본 ```SpringApplication```가 로컬 인스턴스를 대신 생성하는 것을 선호하지 않거나 수정하기를 바랄수도 있다. 예를 들어, 배너를 출력하고 싶지않다면:

```java
public static void main(String[] args) {
    SpringApplication app = new SpringApplication(MySpringConfiguration.class);
    app.setShowBanner(false);
    app.run(args);
}
```

> 노트: ```SpringApplication```으로 전달된 생성인자는 스프링빈을 위한 설정소스다. 대부분의 경우 ```@Configuration```를 참조하지만, XML 설정이나 탐색을 위한 패키지 경로일 수 있다.

```SpringApplication```에 관한 설정은 가능하다면 ```application.properties``` 파일을 사용하자. [23. 외부설정](#외부설정)에서 보다 상세한 내용을 볼 수 있다.

설정 항목들에 대한 완성된 리스트는 [SpringApplication Javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/SpringApplication.html)에서 볼 수 있다.

### 22.3. 플루언트 빌더 API<a name="플루언트 빌더 API"></a>
```ApplicationContext``` 계층(부모/자식 관계의 다양한 컨텍스트)에 관한 빌드가 필요하다거나, '플루언트fluent' 빌더 API 사용을 참조한다면, ```SpringApplicationBuilder```를 사용할 수 있다.

```SpringApplicationBuilder```는 다양한 메서드를 연이어 호출할 수 있고 ```parent```와 ```child``` 메서드를 통해서 계층 생성을 허용한다.

예를 들어:
```java
new SpringApplicationBuilder()
    .showBanner(false)
    .sources(Parent.class)
    .child(Application.class)
    .run(args);
```

> 노트: ```ApplicationContext``` 계층을 생성할 때 몇가지 제약이 있다면, 예를 들어, 웹 컴포넌트는 자식 컨텍스트를 반드시 포함해야 하며 부모와 자식 컨텍스트 모두 같은 ```Envirionment```를 사용해야 한다. 보다 상세한 내용은 [SpringApplicationBuilder javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/builder/SpringApplicationBuilder.html)를 살펴보라.

### 22.4. 애플리케이션 이벤트와 리스너<a name="22.4. 애플리케이션 이벤트와 리스너"></a>
[ContextRefreshedEvent](http://docs.spring.io/spring/docs/4.1.3.RELEASE/javadoc-api/org/springframework/context/event/ContextRefreshedEvent.html)와 같은 스프링 프레임워크 이벤트를 사용한다면, ```SpringApplication```은 몇가지 애플리케이션 이벤트를 추가적으로 전송한다. 어떤 이벤트들은 ```ApplicationContext```가 생성되기 이전에 발생하기도 한다.

이벤트 리스너를 등록하는 방법은 여러가지가 있는데, 가장 일반적인 방법은 ```SpringApplication.addListener(...)``` 메서드를 사용하는 것이다.

애플리케이션 이벤트는 애플리케이션이 실행되면서 다음의 순서로 전송된다.
1. ```ApplicationStartedEvent``` 는 가동되는 순간 전송되지만, 리스너를 등록하고 초기화하는 과정 이전의 과정에 대해서는 제외시킨다.
2. ```ApplicationEnvrionmentPreparedEvent```는 알고 있는 컨텍스트가 ```Environment```를 사용할 떄 전송된다, 단 이전에 컨텍스트는 생성되어 있어야 한다.
3. ```ApplicationPreparedEvent```는 갱신이 시작되기 직전에 전송된다, 단 빈 정의는 적재가 완료되어야 한다.
4. ```ApplicationFailedEvent```는 구동단계에서 예외가 발생했을 때 보낸다.

>팁: 애플리케이션 이벤트를 사용할 필요는 없지만 그것들이 있다는 것을 알아둔다면 편할 것이다. 내부적으로, 스프링부트는 다양한 작업을 다루기 위해 이벤트를 사용한다.

### 22.5. 웹 환경
```SpringApplication```은 사용자를 대신하여 ```ApplicationContext``` 유형을 생성한다. 기본적으로, ```AnnotationConfigApplicationContext``` 혹은 ```AnnotationConfigEmbeddedWebApplicationContext```을 사용할 것이고, 웹 애플리케이션을 사용하거나 그렇지 않을 때도 영향을 받게 된다.

'웹 환경web environment' 사용여부를 정의하는 알고리즘은 매우 간단하다(몇몇 클래스에 영향을 끼쳤다). ```setWebEnvironment(boolean webEnvironment)```를 사용할 수 있으며 필요하다면 기본내용을 오버라이드할 수 있다.

```ApplicationContext``` 유형의 제어를 완벽히 하고 싶다면 ```setApplicationContextClass(...)```를 호출하여 사용할 수 있다.

> 팁: ```setWebEnvirionment(false)는 jUnit 테스트에서 ```SpringApplication``` 사용할 때 자주 사용한다.

### 22.6. 커맨드라인러너 사용
커멘드라인을 통해 전달받은 인자를 접근하고 싶다거나, ```SpringApplication```에서 특정 모드를 실행해야한다면 ```CommandLineRunner``` 인터페이스를 구현하면 된다. ```run(Stirng..args)``` 메서드는 이 인터페이스를 구현한 모든 스프링빈을 호출할 것이다.

```java
import org.springframework.boot.*
import org.springframework.stereotype.*

@Component
public class MyBean implements CommandLineRunner {

    public void run(String... args) {
        // Do something...
    }

}
```

여러가지 ```CommandLineRunner``` 빈을 특정한 순위에 따라서 호출해야한다면, 추가적으로 ```org.springframework.core.Ordered``` 인터페이스를 구현하거나 ```org.springframework.core.annotation.Order``` 애노테이션을 추가한다.

### 22.7. 애플리케이션 종료
각각의 ```SpringApplication``` 은 ```ApplicationContext```가 정상적으로 종료되었는지를 확인하기위해 JVM에 종료 훅Hook을 등록합니다. 모든 기본 스프링 생명주기 콜백(```DisposableBean``` 인터페이스나 ```@PreDestroy``` 애노테이션)을 사용할 수 있다.

추가적으로, ```org.springframework.boot.ExitCodeGenerator``` 인터페이스를 구현한 빈들은 애플리케이션이 종료될 떄 특정 exit code를 반환하기를 원하는 경우 사용한다.

## 23. 외부설정<a name="23. 외부설정"></a>
스프링부트는 동일한 애플리케이션으로 다른 환경에서 동작할 수 있도록 설정을 확장하는 것을 허용한다. 프로퍼티스 파일, YAML 파일, environment 변수 그리고 커맨드라인 인자를 통해서 설정을 확장할 수 있다. 속성 값은 ```@Value``` 애노테이션을 사용하여 바로 주입할 수도, 스프링의 ```Environment``` 추상화에 접근하거나 객체를 구축하여 연동할 수 있다.

스프링부트는 값values, 속성properties 들에 대해서 다음과 같은 순위를 고려하여 합리적으로 오버라이딩하는 것을 허용하도록 설계된 매우 세분화된 ```Pr다opertySource``` 순위order를 사용한다.

> 1. 커맨드라인 인자
> 2. java:comp/env 의 JNDI 어트리뷰트
> 3. 자바 시스템 프로퍼티스(System.getProperties)
> 4. OS 환경 변수
> 5. ```RandomValuePropertySource```의 ```random.*``` 프로퍼티즈
> 6. 포장된 jar 외부의 애플리케이션 프로퍼티즈(YAML과 프로파일 변수를 포함한 application.properties)
> 7. 포장된 jar 내부의 애플리케이션 프로퍼티즈(YAML과 프로파일 변수를 포함한 application.properties)
> 8. ```@Configuration``` 클래스들의 ```@PropertySource``` 애노테이션
> 9. 기본 속성(SpringApplication.setDefaultProperties를 사용하여 정의)

구현예제를 제공하자면, ```name```프로퍼티를 사용하는 ```@Component```를 개발하고 있다고 가정하자:
```java
import org.springframework.stereotype.*
import org.springframework.beans.factory.annotation.*

@Component
public class MyBean {

    @Value("${name}")
    private String name;

    // ...

}
```

jar 에 포함된 ```application.properties```에는 합리적인 기본값으로 ```name```을 제공한다. 출시하여 실행하려할 때, ```application.properties```는 jar 테스트를 위해서 외부에서 ```name```을 오버라이드할 수 있게 해준다. 커맨드 라인에서 변경하여 실행할 수 있다(예: ```java -jar app.jar -name="Spring")

```RandomValuePropertySource```는 무작위 값을 주입하는데 매우 유용하다(예: 시크릿을 넣거나 테스트 작성시). integer, long 혹은 string을 제공한다. 예:

```
my.secret=${random.value}
my.number=${random.int}
my.bignumber=${random.long}
my.number.less.than.ten=${random.int(10)}
my.number.in.range=${random.int[1024,65536]}
```

```random.int*``` 문법은 ```OPEN value(,max) CLOSE```에서 ```OPEN, CLOSE```는 어느 문자나 가능하며 ```value, max는 정수다. 만약 ```max```가 있다면 ```value```는 최소값이 되고 ```max```는 최대값이 된다(배타적인).

### 23.1. 커맨드라인 속성 접근
기본 ```SpringApplication```은 커맨드라인에서 전달받은 인자('--'으로 시작하는, 예: ```--server.port=9000```)를 ```property```로 변환하여 스프링 ```environment```에 추가한다. 앞에서 언급했듯이, 커맨드라인 프로퍼티즈는 다른 프로퍼티 소스들보다 우선한다.

만약 커맨드라인 프로퍼티즈를 ```Environment```에 추가하길 바라지 않는 다면 ```SpringApplication.setAddCommandLineProperties(false)```를 사용하여 비활성화할 수 있다.

### 23.2. 애플리케이션 속성 파일들
```SpringApplication```은 다음 경로들을 순차적으로 탐색하여 ```application.properties``` 파일로부터 프로퍼티즈들을 읽어들여 스프링 ```Envirionment```에 추가할 것이다:

> 1. 현재 디렉토리에서 ```/config``` 하위디렉토리
> 2. 현재 디렉토리
> 3. 클래스패스 상에서 ```/config```패키지
> 4. 클래스패스 루트

목록은 내림차순으로 정렬되었다(목록 상위에 위치한 것들은 하위 아이템들로 덮어쓰인다).
> 노트: '.properties' 대신에 [YAML('.yaml') 파일을 사용](#Properties 대신 YAML 사용)할 수 있다.

```applicaiton.properties```를 설정파일 이름으로 선호하지 않는다면 ```spring.config.name``` 환경속성을 정의하여 변경할 수 있다. 혹은 ```spring.config.location``` 환경속성을 사용하여 위치를 명확하게 정의할 수도 있다(콤마 구분자(,)를 사용하여 디렉토리 위치나 파일의 경로를 다수 적용가능하다)

```
$ java -jar myproject.jar --spring.config.name=myproject
```

혹은

```
$ java -jar myproject.jar --spring.config.location=classpath:/default.properties,classpath:/override.properties
```

만약 ```spring.config.location``` 에 포함된 디렉토리들(혹은 파일들로 등록한 경우)이 ```/```로 끝난다면 적재하기 전에 ```spring.config.name```을 이용하여 뒤에 이름을 붙일 것이다. 기본 탐색 경로는 ```classpath:,classpath:/config,file:,file:config/``` 을 항상 사용하며, ```spring.config.location```의 값을 포함한다.

### 23.3. <a name='프로파일 지정 속성들'>프로파일 지정 속성들</a>
```application.properties``` 파일에 추가적으로, 프로퍼티스파일에 프로파일을 지정할 수 있는데 ```application-{profile}.properties``` 형식으로 작명관례를 사용하여 정의하면 된다.

### 23.4. 속성 플레이스홀더(placeholder)
```applicaton.properties```의 값들은 ```Environment```가 존재하는 경우 걸러지게 되는데, 그 과정을 이용하여 앞에서 정의한 값을 뒤에서 참조할 수 있다(예, 시스템 프로퍼티스).
```
app.name=MyApp
app.description=${app.name} is a Spring Boot application
```

> 팁: 스프링부트에 있는 프로퍼티스들을 축약하여 기술적으로 사용할 수 있다. 이와 관련해서는 [64.3. '간략한' 커맨드라인 인자 사용](#'간략한' 커맨드라인 인자 사용)에서 어떻게 사용하는지 상세한 설명을 볼 수 있다.

### 23.5. Properties 대신 YAML 사용<a name="23.5. Properties 대신 YAML 사용"></a>
[YAML](http://yaml.org/)은 JSON에 포함되며 계층적인 설정 데이터를 정의하는데 매우 편리한 문법을 가지고 있다. ```SpringApplication``` 클래스는 클래스패스 상에 [SnakeYAML]()라이브러리를 가지고 있다면 YAML을 지원할 수 있도록 프로퍼티스에서 자동전환한다.

> 노트: ```spring-boot-starter```에서는 자동으로 ```SnakeYAML``` 'starter POM`'를 제공한다.

#### 23.5.1. YAML 읽어오기
스프링부트는 YAML 문서를 읽어와서 사용하는데 편의를 제공하는 두개의 클래스를 제공한다. ```YamlPropertiesFactoryBean```은 YAML을 ```Properties``` 처럼 읽어오고 ```YamlMapFactoryBean```은 YAML을 ```Map```처럼 읽어온다.

예를 들어, 다음과 같은 YAML 문서가 있다:
```
environments:
    dev:
        url: http://dev.bar.com
        name: Developer Setup
    prod:
        url: http://foo.bar.com
        name: My Cool App
```

위 항목을 properties로 변환하면 다음과 같다:
```
environments.dev.url=http://dev.bar.com
environments.dev.name=Developer Setup
environments.prod.url=http://foo.bar.com
environments.prod.name=My Cool App
```

YAML 목록은 ```[index]``` 참조를 가지는 프로퍼티 키로서 표현된다. YAML 예제:
```
my:
   servers:
       - dev.bar.com
       - foo.bar.com
```

를 properties로 변환하면 다음과 같다:
```
my.servers[0]=dev.bar.com
my.servers[1]=foo.bar.com
```

properties가 연결되는 것처럼 스프링 ```DataBinder``` 유틸리티를 사용할 수 있다(```@ConfigurationProperties``` 가 어떻게 동작하는지 살펴보라) 대상이 되는 빈에서 ```java.util.List(or Set)``` 속성을 가지고 씨거나 혹은 수정자(setter)를 사용하거나, 변경될 수 있는 값(예를 들어, 위에서 본 프로퍼티스도 유사하게 연결)을 초기화할 수도 있다.

```
@ConfigurationProperties(prefix="my")
public class Config {
    private List<String> servers = new ArrayList<String>();

    public List<String> getServers() {
        return this.servers;
    }
}
```
#### 23.5.2. 스프링 환경에서 속성들을 YAML로 노출
```YamlPropertySourceLoader``` 클래스는 스프링 ```Environment```의 ```PropertySource````처럼 외부의 YAML을 사용할 수 있다. 이는 YAML 속성들에 접근하기 위한 플레이스홀더 문법인 ```@Value``` 애노테이션과 유사한 형태로 사용하는 것을 허용한다.

#### 23.5.3. 다중 프로파일 YAML 문서
단독 파일로 구성된 YAML 문서에 ```spring.profiles```키로 지정항 다중 프로파일을 저으이하여 사용하는 것이 가능하다. 예를 들어:
```
server:
    address: 192.168.1.100
---
spring:
    profiles: development
server:
    address: 127.0.0.1
---
spring:
    profiles: production
server:
    address: 192.168.1.120
```

위의 예에서, ```server.address``` 속성이 ```127.0.0.1```라면 ```development```` 속성이 활성화 상태다. 만약 ```development``` 와 ```production``` 프로파일을 사용할 수 **없다면**, 속성값은 ```192.168.1.100```일 것이다.

#### 23.5.4. YAML 의 단점
YAML 파일은 ```@PropertySource``` 애노테이션 등으로 불러올 수 없다. 이와 같은 형태로 값을 호출하여 사용해야 프로퍼티스 파일을 사용해야 한다.

### 23.6. 타입세이프 설정 속성들
```@Value("${property}")``` 애노테이션을 사용하여 설정 속성을 주입받아 사용하는 것이 번거로운 경우가 있다. 다중 속성을 이용하여 작업하거나 계층 구조의 데이터을 다루게 되는 경우가 그렇다. 스프링부트는 허용된 강력한 타입 빈즈들에서 사용가능한 속성들을 선택할 수 있는 메서드를 제공하고 애플리케이션의 설정에 관해 검증한다. 예를 들어:

```
@Component
@ConfigurationProperties(prefix="connection")
public class ConnectionSettings {

    private String username;

    private InetAddress remoteAddress;

    // ... getters and setters

}
```

```@EnableConfigurationProperties``` 애노테이션은 ```@Configuration```을 포함한다, ```@ConfigurationProperties```가 선언된 빈은 자동적으로 ```Environment``` 속성이 설정된다. 이런 설정 유형은 ```SpringApplication``` 확장 YAML 설정을 사용할 경우에만 적용된다.

```
# application.yml

connection:
    username: admin
    remoteAddress: 192.168.1.1

# additional configuration as required
```

```@ConfigurationProperties``` 가 적용된 빈즈는 다음에서 보게되는 빈의 형태로 주입된다.

```java
@Service
public class MyService {

    @Autowired
    private ConnectionSettings connection;

     //...

    @PostConstruct
    public void openConnection() {
        Server server = new Server();
        this.connection.configure(server);
    }

}
```

또한 ```@EnableConfigurationProperties``` 애노테이션을 사용하여 프로퍼티스 클래스 목록을 정의한 ```@ConfigurationProperties``` 빈을 간단하게 등록할 수도 있다.

```
@Configuration
@EnableConfigurationProperties(ConnectionSettings.class)
public class MyConfiguration {
}
```

#### 23.6.1. 느슨한 연결
스프링부트는 ```@ConfigurationProperties``` 빈에 대한 ```Envirionment``` 속성연결을 느슨하게 정의하여 사용한다, 또한 ```Environment``` 속성명과 빈의 속성명을 정확하게 맞춰줄 필요도 없다. 일반적인 예로 언더스코어('_') 구분자를 포함하거나(예, ```context_path```는 ```contextPath```에 연결), 그리고 대소문자(예, ```PORT```는 ```port```에 연결) 환경속성들에서 유용하게 적용된다.

스프링은 ```@ConfigurationProperties``` 빈이 바인딩될 때 적절한 형식으로 외부 애플리케이션 속성을 적용하려고 시도한다. 별도유형의 컨버전이 필요하다면 ```ConversionService``` 빈(```conversionService``` 빈 아이디) 혹은 별도의 프로퍼티 에디터를 제공할 수 있다.

#### 23.6.2. ```@ConfigurationProperties``` 검증
스프링부트는 외부 설정에 관한 JSR-303(클래스패스 상에 있다면)을 이용한 검증을 제공한다. JSR-303 ```javax.validation``` 제약 어노테이션을 ```@ConfigurationProperties``` 클래스에 추가하면 사용할 수 있다.

```
@Component
@ConfigurationProperties(prefix="connection")
public class ConnectionSettings {

    @NotNull
    private InetAddress remoteAddress;

    // ... getters and setters

}
```

또한 ```configurationPropertiesValidator```이라 불리는 빈 정의를 생성하면 커스텀 스프링 ```Validator```를 추가할 수 있다.
> 팁: ```spring-boot-actuator``` 모듈은 모든 ```@ConfigurationProperties``` 빈들을 탐색할 수 있는 엔드포인트를 포함하고 있다. 간단하게 브라우저에서 ```/configprops```로 접근하거나 이와 동등한 JMX 엔드포인트를 사용할 수 있다. 이와 관련해서는 보다 자세한 사항은 [출시준비 기능](#엔드포인트) 섹션을 살펴보기 바란다.

## 24. 프로파일<a name="24. 프로파일"></a>
스프링 프로파일즈는 독립된 환경 속에서 명확한 환경 속에서 애플리케이션의 설정을 관리할 수 있도록 분리하는 방법을 제공하고 있다. 어느 ```@Conponent``` 혹은 ```@Configuration``` 이든 ```@Profile```을 지정하여 읽어오는 것을 제한할 수 있다:

```java
@Configuration
@Profile("production")
public class ProductionConfiguration {

    // ...

}
```

보통의 스프링이 제공하는 방법으로는, ```spring.profiles.active Environment``` 속성을 통해서 프로파일즈를 활성화할 수 있다. 속성에서 지정하는 일반적인 방법으로는, 다음의 예제에서 처럼 ```applicatoin.properties``` 안에 포함시킬 수 있다:
```
spring.profiles.active=dev,hsqldb
```

혹은 커맨드라인에서 ```--spring.profiles.active=dev,hsqldb```와 같이 사용하여 변환을 지정할 수 있다.

### 24.1. 활성프로파일 추가
```spring.profiles.active``` 속성은 다른 프로퍼티즈의 우선순위 정책을 동일하게 따른다. 가장 우선순위가 높은 ```PropertySource```가 승리한다. 이것이 의미하는 것은 ```application.properties```에 지정된 지정된 활성프로파일즈는 커맨드라인 스위치를 사요하면 그것으로 대체된다.

때때로 프로퍼티즈에 정의된 프로필을 다른 것으로 대체하는 것보다 활성 프로파일즈를 **추가** 하는 방법이 유용할 수 있다. ```spring.profiles.include``` 속성을 이용하면 별다른 조건없이 활성프로파일즈를 추가할 수 있다. ```SpringApplication``` 진입점(엔트리포인트)의 설정을 위한 Java API를 프로파일즈를 추가설정할 수 있다(예를 들어, ```spring.profiles.active``` 속성은 최상위에서 활성화된다): ```setAdditionalProfiles()``` 메서드를 살펴보길 바란다.

예를 들어, 애플리케이션의 다음에 있는 프로퍼티즈와 함께 ```--spring.profiles.active=prod``` 스위치를 사용하여 실행하면 ```proddb```와 ```prodmq```가 함께 활성화될 것이다.

```
---
my.property: fromyamlfile
---
spring.profiles: prod
spring.profiles.include: proddb,prodmq
```

> 노트: ```spring.profiles``` 속성을 YAML 문서에 정의할 때 이 문서의 설정을 포함한 부분들을 분리시키는 구분자를 기억할 것이다. 보다 자세한 내용은 [64.6 "환경 의존적 설정 변경"](#환경 의존적 설정 변경)을 살펴보자.

### 24.2. 프로파일 작성방법
애플리케이션이 실행되기 전에 ```SpringApplication.setAdditionalProfiles(…​)``` 를 호출하여 프로그램적으로 활성프로파일즈를 설정할 수 있다. 이는 스프링의 ```ConfigurableEnvironment``` 인터페이스를 사용해서 활성 프로파일즈 설정이 가능하다.

### 24.3. 프로파일 상세 설정파일
프로파일 정의의 변형은 ```application.properties```(혹은 ```application.yml```) 그리고 ```@ConfigurationProperties``` 를 통해서 파일들을 적재하는 경우를 고려해볼 수 있다. 보다 자세한 내용은 [23.3 "프로파일 지정 속성들"](#프로파일 지정 속성들)을 살펴보기 바란다.

## 25. 로깅<a name="로깅"></a>
스프링부트는 모든 내부 로깅에 [Commons Logging](http://commons.apache.org/logging)를 사용한다, 그러나 근원적인 로그 구현체를 열어볼 수 있다. 기본 설정들은 [Java Util Logging)(http://docs.oracle.com/javase/7/docs/api/java/util/logging/package-summary.html), [Log4j](http://logging.apache.org/log4j/) 그리고 [Logback](http://logback.qos.ch/)을 제공한다. 각각 콘솔로 출력되고 파일로
출력된다(10MB 크기가 되면 파일을 새로 생성).

기본적으로, 'Starter POMs'를 사용한다면, Logback을 로깅에 사용할 것이다. 유연한
 Logback은 Java Util Logging, Commons Logging, Log4j 혹은 SLF4J 를 사용하는 의존적 라이브러리들을 의존적인 라이브러리들도 문제없이 동작하는 것을 보장한다.
 > 팁:
 > 자바에서 사용가능한 로깅 프레임워크들은 대부분 지원한다. 목록만 보고서 당혹러워할 이유는 없다. 기본적으로 로깅 의존성을 변경할 필요는 없을 것이며 스프링부트는 기본적으로 잘 되어 있어있다.

### 25.1. 로그 형식
스프링부트의 기본적인 로그 출력은 다음과 같다:
```
2014-03-05 10:57:51.112  INFO 45469 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet Engine: Apache Tomcat/7.0.52
2014-03-05 10:57:51.253  INFO 45469 --- [ost-startStop-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2014-03-05 10:57:51.253  INFO 45469 --- [ost-startStop-1] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 1358 ms
2014-03-05 10:57:51.698  INFO 45469 --- [ost-startStop-1] o.s.b.c.e.ServletRegistrationBean        : Mapping servlet: 'dispatcherServlet' to [/]
2014-03-05 10:57:51.702  INFO 45469 --- [ost-startStop-1] o.s.b.c.embedded.FilterRegistrationBean  : Mapping filter: 'hiddenHttpMethodFilter' to: [/*]
```

출력된 로그에 포함된 정보는 다음과 같다:
* 날짜와 시간 - 밀리세컨드ms 단위로 꼼꼼하고 쉽게 정렬가능하다.
* 로그레벨 - ```ERROR```, ```WARN```, ```INFO```, ````DEBUG``` 그리고 ```TRACE```
* 프로세스 ID
* ```---``` - 실제 로그메시지가 출력되는 부분을 나누려는 구분자
* Logger name - 소스 클래스 네임(자주 줄어든다).
* 로그 메시지

### 25.2. 콘솔 출력
기본 로그 설정은 각각의 메시지가 콘솔에 출력된다. 기본적으로 ```ERROR```, ```WARN``` 그리고 ```INFO``` 레벨 메시지가 출력된다. 또한 ```DEBUG``` 레벨 메시지는 애플리케이션을 실행할 때 ```--debug``` 프래그와 함께 실행하면 출력된다.
```
$ java -jar myapp.jar --debug
```

터미널에서 ANSI를 지원한다면, 칼라로 출력되며 가독성을 높여줄 것이다. ```spring.output.ansi.enabled``` 를 정의하여 [제공값](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/ansi/AnsiOutput.Enabled.html)을 덧씌울 수 있다.

### 25.3. 파일 출력
기본적으로, 로그파일은 실행환경에 정의된 ```temp``` 디렉토리에 ```spring.log``` 라는 이름으로 기록되며, 10MB 단위로 생성된다. 로그 생성 폴더는 ```logging.path``` 속성(```application.properties``` 를 예로 들자면)을 설정하여 쉽게 변경가능하다. 또한 ```logging.file``` 속성을 이용해서 파일명을 변경하는 것도 가능하다.

> 노트: 만약 ```logging.file```을 사용한다면, ```loggging.path``` 설정은 적용되지 않는다.

콘솔에 출력되는 것은 ```ERROR```, ```WARN``` 그리고 ```INFO``` 레벨의 메시지가 기본출력된다.

### 25.4. 로그 레벨

스프링 ```Environment```(예를 들어 ```applicatoin.properties```)에 ```logging.leve.*=Level```로 정의하고 ```LEVEL```에는 ```TRACE```, ```DEBUG```, ```INFO```, ```WARN```, ```ERROR```, ```FATA```, ```OFF``` 중에서 선택하면 로그 레벨은 모든 지원가능한 로깅 시스템에 적용된다. ```application.properties``` 예제로:

```
logging.level.org.springframework.web: DEBUG
logging.level.org.hibernate: ERROR
```

### 25.5. 로그 설정 변경<a name="로그 설정 변경"></a>

다양한 로깅 시스템은 기본적인 라이브러리를 포함하여 클래스패스 상의 활동상태를 관찰할 수 있다, 또한 클래스패스 루트에 위치한 적절한 설정파일을 제공하면 변경할 수 있으나, 스프링 ```Environment``` ```logging.config``` 속성으로 정의해야한다. (보충하자면, 로깅 시작은 ```ApplicationContext```가 **생성되기 전** 초기화되는 순간부터 시작된다. 스프링 ```@Configuration``` 파일에서 ```@PropertySources``` 에서 로깅을 컨트롤하는 것은 불가능하다. 시스템 프로퍼티즈와 스프링부트의 외부설정 파일을 이용한 것은 잘 동작한다. )

로깅시스템의 부수적인, 다음의 파일들이 있어야 한다:

| 로깅 시스템 | 설정파일 |
|------------|----------|
| Logback | logback.xml |
| Log4j | log4j.properties 혹은 log4j.xml |
| JDK(Java Util Logging) | logging.properties |

설정에 필요한 몇몇 속성들은 스프링 ```Envirionment```에서 시스템 프로퍼티스로 변환된다.

| Spring environment | System property | 설명 |
|--------------------|-----------------|------|
| logging.file | LOG_FILE | 정의되어 있다면 기본 로그 설정으로 사용된다. |
| lggging.path | LOG_PATH | 정의도어 있다면 기본 로그 설정으로 사용된다. |
| PID | PID | 현재 프로세스 ID(가능하다면 발견한 프로세스 ID를 사용하며 정의되어 있지 않은 경우에는 OS 환경 변수를 사용한다.) **재확인** |

모든 로깅 시스템에 대한 지원은 로깅 시스템의 설정 파일을 분석하여 시스템 프로퍼티스로 변환할 수 있기 때문이다. 예제로 ```spring-boot.jar``` 안에 기본 설정을 살펴보라.
> 위험: 실행가능한 JAR로 실행했을 때 Java Util Logging을 사용할 때 클래스로딩classloading 에서 문제가 발생한다는 이슈가 있다. 우리는 가능하면 이것을 피하기를 권장한다.

## 26. 웹 애플리케이션 개발
스프링부트는 웹 애플리케이션 배포에 최적화되어 있다. 내장형 톰캣tomcat, 제티jetty 혹은 언더토우Undertow 등을 사용한 내장형 HTTP 서버를 쉽게 만들 수 있다. ```spring-boot-starter-web``` 모듈을 사용하여 웹 애플리케이션을 빠르게 구성하고 실행할 수 있다.

만약 스프링부트 웹 애플리케이션을 개발해본 경험이 없다면 [시작하기](#초기 스프링부터 애플리케이션 개발)섹션의 "Hello world!" 예제를 따라할 수 있다.

### 26.1. 'Spring Web MVC framework'<a name="Spring Web MVC framework"></a>

스프링 웹 MVC 프레임워크(줄여서 'Spring MVC')는 강력한 '모델 뷰 컨트롤러' 웹 프레임워크다. 스프링MVC 는 특별한 ```@Controller```혹은 ```@RestController``` 빈을 생성하여 HTTP 요청을 다룰 수 있다. 컨트롤러의 메서드는 ```@RequestMapping``` 어노테이션을 사용하여 HTTP에 매핑할 수 있다.

여기 **JSON** 데이터를 제공하는 기본적인 ```@RestController``` 예제가 있다:
```
@RestController
@RequestMapping(value="/users")
public class MyRestController {

    @RequestMapping(value="/{user}", method=RequestMethod.GET)
    public User getUser(@PathVariable Long user) {
        // ...
    }

    @RequestMapping(value="/{user}/customers", method=RequestMethod.GET)
    List<Customer> getUserCustomers(@PathVariable Long user) {
        // ...
    }

    @RequestMapping(value="/{user}", method=RequestMethod.DELETE)
    public User deleteUser(@PathVariable Long user) {
        // ...
    }

}
```

스프링MVC는 코어 스프링프레임워크의 일부이며 자세한 정보는 [레퍼런스 문서](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle#mvc)에서 얻을 수 있다. [spring.io/guides](http://spring.io/guides)에서 스프링MVC를 지원하는 다양한 가이드를 살펴볼 수 있다.

#### 26.1.1. Spring MVC 자동설정
스프링부트는 대부분의 애플리케이션에서 동작하는 스프링MVC에 관한 자동설정을 제공한다.

자동설정은 스프링이 기본적으로 제공하는 최상의 기능들을 추가한다:
* ```ContentNegotiatingViewResolver```와 ```BeanNameViewResolver``` 빈을 포함
* Webjars지원을 포함한 정적 자원 제공을 지원(추가내용 제공)
* ```Converter, GenericConverter, Formatter``` 빈을 자동등록
* ```HttpMessageConverters``` 지원(추가내용 제공)
* ```MessageCodeResolver``` 자동 등록(추가내용 제공)
* 정적 ```index.html``` 지원
* ```favicon``` 변경 지원

스프링MVC을 완벽히 제어하고 싶다면, ```@Configuration``` 와 함께 ```@EnableWebMvc``` 를 사용할 수 있다. 만약 스프링부트 MVC 기능을 사용하지 않고, 추가적인 [MVC 설정](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle#mvc)으로 (인터셉터interceptors, 포맷터formatters, 뷰view 컨트롤러 등)
```WebMVcConfigureAdapter``` 유형의 ```@Bean```을 추가할 수 있다. ```@EnableWebMvc```**없이**.

#### 26.1.2. ```HttpMessageConverter```
스프링MVC는 HTTP 요청과 응답을 변환하는데 ```HttpMessageConverter``` 인터페이스를 사용한다. 기본적으로 제공하는 설정은, 예를 들어 객체는 자동으로 JSON(Jackson 라이브러리를 사용) 이나 XML(가능하다면 Jackson XML 확장을 사용하거나 JAXB를 사용)으로 변환한다. 문자열string은 ```UTF-8```로 기본 인코딩된다.

만약에 컨버터를 추가하거나 수정하려 한다면 스프링부트에서 ```HttpMessageConverter``` 클래스를 사용할 수 있다:
```
import org.springframework.boot.autoconfigure.web.HttpMessageConverters;
import org.springframework.context.annotation.*;
import org.springframework.http.converter.*;

@Configuration
public class MyConfiguration {

    @Bean
    public HttpMessageConverters customConverters() {
        HttpMessageConverter<?> additional = ...
        HttpMessageConverter<?> another = ...
        return new HttpMessageConverters(additional, another);
    }

}
```

```HttpMessageConverter``` 빈은 컨텍스트에 컨버터 목록을 추가할 것이다. 또한 기본 컨버터들을 덧칠override 하는 방법도 있다.

#### 26.1.3. ```MessageCodesResolver```
스프링MVC는 ```MessageCodeConverter```에 선언된 에러로부터 에러메시지를 표시하기 위해 에러코드를 생성하는 전략을 가지고 있다. ```spring.mvc.message-codes-resolver.format```를 설정하여 ```PREFIX_ERROR_CODE``` 혹은 ```PREFIX_ERROR_CODE``` 속성을 설정해뒀다면 스프링부트가 ```MessageCodesResolver```를 생성할 것이다(```DefaultMessageCodesResolver.Format``` 목록을 살펴보자 ).

#### 26.1.4. 정적 컨텐츠Static Content
스프링부트는 기본적으로 클래스패스 혹은 ```ServletContext``` 루트에 있는 ```/static```(혹은 ```/public``` 혹은 ```/resource``` 혹은 ```/META-INF/resource```) 기반으로 정적 컨텐츠를 제공한다. 스프링MVC의 ```ResourceHttpRequestHandler```를 사용하거나 ```WebMvcConfigureAdapter```를 추가하고 ```addResourceHandler``` 메서드를 오버라이드하여 수정할 수 있다.

스프링에서 정적 컨텐츠를 다루지 않기로 설정되어 있다면, 독립 수행 웹 애플리케이션의 기본 서블릿은 ```ServletContext``` 루트에서 컨텐츠를 제공하는 등의 기능을 수행할 것이다. 그러나 기본 MVC 설정을 변경하지 않는한 이런 일은 거의 없다. 스프링은 가능하다면 모든 요청을 ```DispatcherServlet```을 통해서 제어하려고 한다.

앞에서 살펴본 ```기본``` 정적 자원 위치 외에, [Webjars content](http://www.webjars.org/) 를 사용하는 특이한 경우가 있다. **Webjar** 형태로 묶인 jar 파일 안에 있는 ```/webjars/**``` 경로에 있는 자원들이 제공된다.

> 팁: 애플리케이션을 **jar** 로 묶으려packaged 한다면 ```src/main/webapp``` 폴더는 사용하지 말자. 이 폴더는 일반적으로, **'war' 묶음인 경우에만** 동작하며, 대부분의 빌드툴이 **jar** 파일을 생성하는 과정에서 암묵적으로 무시한다.

#### 26.1.5. Template engines
REST 웹서비스가 잘 되어 있다면, 스프링MVC를 이용하여 동적인 HTML 컨텐츠를 제공할 수 있다. 스프링MVC는 벨로시티Velocity, 프리마커FreeMarker 그리고 JSP 등을 포함한 다양한 템플릿 기술을 지원한다. 다양한 템플릿 엔진들을 스프링MVC와의 통합된다.

스프링부트는 다음의 템플릿 엔진들을 지원하는 자동설정을 포함하고 있다:
* [프리마커FreeMarker](http://freemarker.org/docs/)
* [그루비Groovy](http://beta.groovy-lang.org/docs/groovy-2.3.0/html/documentation/markup-template-engine.html)
* [타임리프Thymeleaf](http://www.thymeleaf.org/)
* [벨로시티Velocity](http://velocity.apache.org/)

위에 거론된 템플릿 엔진들 중에서 한가지를 기본설정으로 사용하며느, 템플릿들은 ```src/main/resources/template``` 에서 자동으로 가져온다.

> 팁: JSPs는 가능하면, 내장형 서블릿 컨테이너를 사용할 때 [알려진 여러가지 제약사항들](file:///home/honeymon/workspace/git-repository/translate-spring-boot-reference-doc/Spring%20Boot%20Reference%20Guide.html#boot-features-jsp-limitations)을 피하길 바란다.

#### 26.1.6. 오류 제어Error handling
스프링부트는 ```/error``` 와 매칭되는 다양한 경로의 모든 에러 서블릿 컨테이너에 등록된 'global' 에러 페이지를 제어한다. 클라이언트는 HTTP 상태와 예외 메시지 등의 에러에 관한 자세한 내용을 JSON 응답으로 제공받을 수 있다. 브라우저인 경우에는 HTML 형태에 동일한 데이터를 기록한 `Whitelabel!`(변경하는 방법려면 'error'를 처리하는 ```view```를 추가하면 된다) 에러 뷰를 보게된다. 기본적으로는 ```ErrorController```를 구현하고 빈으로 저의하면 완벽히 대처가 가능하다. 혹은 이미 존재하는 기작에 따라 ```ErrorAttributes``` 빈을 간단히 추가할 수 있지만 내용을 대체해야 한다.

몇몇 상황들에 대한 에러페이지를 세밀하게 정의하고자 한다면, 내장형 서블릿 컨테이너는 에러를 제어하기 위한 지원하는 공통uniform 자바 DSL을 제공한다. 예를 들어:

```
@Bean
public EmbeddedServletContainerCustomizer containerCustomizer(){
    return new MyCustomizer();
}

// ...

private static class MyCustomizer implements EmbeddedServletContainerCustomizer {

    @Override
    public void customize(ConfigurableEmbeddedServletContainer container) {
        container.addErrorPages(new ErrorPage(HttpStatus.BAD_REQUEST, "/400"));
    }

}
```

또한 [@ExceptionHandler method](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#mvc-exceptionhandlers) 그리고 [@ControllerAdvice](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#mvc-ann-controller-advice) 같은 일반적인 스프링MVC의 기능들을 사용할 수 있다. ```ErrorController``` 제어되지 않는 예외들을 다룰 때 사용한다.

N.B.(?? 뭐지) ```Filter```를 통해 ```ErrorPage``` 경로를 등록하여 제어할 수도 있다(예로, Jersey 그리고 Wicket 과 같은 비 스프링웹프레임워크에서는 일반적으로 사용), ```Filter```는 ```ERROR``` 디스패쳐dispatcher에 등록된다. 예:

```
@Bean
public FilterRegistrationBean myFilter() {
    FilterRegistrationBean registration = new FilterRegistrationBean();
    registration.setFilter(new MyFilter());
    ...
    registration.setDispatcherTypes(EnumSet.allOf(DispatcherType.class));
    return registration;
}
```

(기본적으로 ```FilterRegisterBean```는 ```ERROR``` dispatcher 타입에 포함되지 않는다)

#### 웹스피어 애플리케이션 서버에서 오류 제어
> 패쓰!!

### 26.2. JAX-RS 그리고 Jersey
REST 엔드포인트르 위해서 JAX-RS 프로그래밍 모델을 참조하여 스프링MVC를 대체할 구현체를 찾고 있다면, 애플리케이션 컨텍스트에 등록되는 ```@Bean``` 처럼 ```Servlet```과 ```Filter```를 등록하면 Jersy 1.x 와 Apache Celtix에서도 잘 동작할 것이다. Jersey 2.x 는 스프링을 지원하기에 스프링부트 스타터에 자동설정을 제공하고 있다.

Jersey 2.x 을 시작할 때 ```spring-boot-starter-jersey``` 스타터에 대한 의존성을 추가하고 ```ResourceConfig``` 형태의 ```@Bean```이 하나 필요하며 여기에 모든 엔드포인트를 등록하면 된다:

```
@Component
public class JerseyConfig extends ResourceConfig {
    public JerseyConfig() {
        register(Endpoint.class);
    }
}
```

등록된 모든 엔드포인트에는 HTTP 자원 애노테이션 종류인 ```@Component```(예: ```@GET```) 가 선언되어야 한다.

```
@Component
@Path("/hello")
public class Endpoint {

    @GET
    public String message() {
        return "Hello";
    }

}
```

```EndPoint```는 ```@Autowired``` 의존성 과 ```@Value``` 를 이용하여 외부설정을 주입하는 등 스프링```@Component```처럼 스프링이 생명주기를 관리한다. Jersy 서블릿은 기본적으로 ```'/*'``` 와 매핑되어 등록된다. 매핑을 변경하고 싶다면 ```ResourceConfig```에 ```@ApplicationPath```를 추가하면 된다.

Jersey는 기본적으로 ```@Bean``` 형태의 "jerseyServletRegistration"이란 이름의 ```ServletRegistrationBean``` 서블릿을 생성한다. 비활성화하거나 동일한 이름의 빈을 오버라이드 하여 생성할 수 있다. 서블릿으로 하는 설정대신 필터를 사용할 수 있다. ```spring.jersey.type=filter```("jerseyFilterRegistration"을 오버라이드 하거나 ```@Bean```을 대체). 서블릿이 가지고 있는 ```@Order```에 대해서는 ```spring.jersey.filter.order```으로 설정할 수 있다. 서블릿과 필터 등록을 할 때 프로퍼티즈에 ```spring.jersey.init.*``` 을 선언하여 초기화 파라메터를 전달할 수 있다.

[jersey 예제](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-jersey)를 보면서 어떻게 설정할 지 살펴볼 수 있을 것이다. [Jersey 1.x 예제](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-jersey1)도 있다. Jersey 1.x 예제 노트에는 스프링부트 메이븐 플러그인을 이용해서 몇몇 Jersey jars를 압축해제하여 JAX-RS 구현체를 스캔하도록 설정하는 것을 설명한다(```Filter``` 등록을 스캔하는 방법의 예제를 살펴볼 수 있다). 내장된 Jars 패키지 안에서 JAX-RS 리소스들도 살펴볼 수 있다.

### 26.3. <a name="내장형 서블릿 컨테이너 지원">내장형 서블릿 컨테이너 지원</a>
스프링부트는 내장형 톰캣Tomcat, 제티Jetty, 그리고 언더토우Undertow 서버를 지원한다. 대부분의 개발자들은 '스타터Starter POM'을 포함시키는 것으로 모든 설정이 되어 있어 쉽게 사용할 수 있다. 내장된 서버의 기본 HTTP Request 접근포트는 **8080** 이다.

#### 26.3.1. 서블릿 그리고 필터
내장형 서블릿 컨테이너를 사용할 때 스프링빈으로 서블릿과 필터를 등록할 수 있다. 설정을 하는 동안 ```application.properties```에서 필요한 값들을 참조할 수 있다.

기본적으로, 단독 서블릿인 경우 컨텍스트는 ```/```에 매핑된다. 다중 서블릿을 사용하는 경우에는 빈의 이름을 경로접두사로 사용할 것이다. 필터는 ```/*```로 매핑된다.

관례적인 매핑으로는 유연함에 부족함을 느낀다면 완벽한 제어를 위해서 ```ServletRegistrationBean``` 그리고 ```FilterRegsitrationBean``` 클래스를 사용할 수 있다. ```ServletContextInitializer``` 인터페이스를 직접 구현하여 등록할 수도 있다.

#### 26.3.2. ```EmbeddedWebApplicationContext```

스프링부트는 내장형 서블릿 컨테이너를 지원하기 위해 ```ApplicationContext```의 새로운 형태를 사용한다. ```EmbbeddedWebApplicationContext```는

#### 26.3.3. 내장형 서블릿 컨테이너 변경
공통 서블릿 컨테이너 설정은 스프링 ```Environment``` 프로퍼티즈를 사용하여 설정할 수 있다. ```application.properties``` 파일에 정의한 프로퍼티즈를 사용한다.

공통 서버 설정에 포함된 내용은:
* ```server.port``` - HTTP 요청 수용 포트
* ```server.address``` - 연결된 인터페이스 주소
* ```server.sessionTimeout``` - 세션 타임아웃

전체목록은 [ServerProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/web/ServerProperties.java) 클래스를 살펴보자.

#### 프로그래밍으로 변경하기
내장 서블릿 컨테이너의 설정을 프로그램적으로 설정할 필요가 있을 경우에는 ```EmbeddedServletContainerCustomizer``` 인터페이스를 구현한 스프링빈을 등록해야한다. ```EmbeddedServletContainerCustomizer```는 변경가능한 다양한 세터 메서드를 가지고 있는 ```ConfigurableEmbeddedServletContainer``` 에 대한 접근을 제공한다.

```
import org.springframework.boot.context.embedded.*;
import org.springframework.stereotype.Component;

@Component
public class CustomizationBean implements EmbeddedServletContainerCustomizer {

    @Override
    public void customize(ConfigurableEmbeddedServletContainer container) {
        container.setPort(9000);
    }

}
```

#### ```ConfigurableEmbeddedServletContainer``` 직접 변경
만약 설정기술이 너무 제한적이라면, ```TomcatEmbeddedServletContainerFactory```, ```JettyEmbeddedServletContainerFactory``` 혹은 ```UndertowEmbeddedServletContainerFactory``` 빈을 등록하는 방법도 있다.

```
@Bean
public EmbeddedServletContainerFactory servletContainer() {
    TomcatEmbeddedServletContainerFactory factory = new TomcatEmbeddedServletContainerFactory();
    factory.setPort(9000);
    factory.setSessionTimeout(10, TimeUnit.MINUTES);
    factory.addErrorPages(new ErrorPage(HttpStatus.404, "/notfound.html");
    return factory;
}
```

세터들은 많은 설정옵션들을 제공한다. 여러 protected 메서드 'hooks'는 보다 다양한 이국적인 기능들을 제공한다. 보다 자세한 내용은 소스코드 문서를 살펴보라.

#### 26.3.4. JSP 제약사항
스프링부트를 실행할 때 내장 서블릿 컨테이너를 사용한다면(실행가능한 압축패키지라면), JSP 지원이 제약되는 경우가 있다.
* 톰캣에서 'war' 패키징을 사용한다면, 실행가능한 war로 동작한다면, 표준 컨테이너에 배포한다면 별다른 문제는 없을 것이다(제한은 없다, 톰캣을 포함해서). 실행가능한 jar 는 톰캣에서 하드코드 파일패턴 때문에 동작하지 않는다.
* 제티는 내장 컨테이너에서 JSP를 지원하지 않는다.
* 언더토우는 JSP를 지원하지 않는다.

## 27. <a name="보안">보안</a>
스프링시큐리티는 웹 애플리케이션의 모든 HTTP 엔드포인트들에 대한 '기초'적인 인증을 기본적인 보안을 처리한다. 웹 애플리케이션에 메서드-레벨의 보안을 추가하려면 ```@EnableGlobalMethodSecurity``` 를 설정에 추가하면 된다. 추가적인 정보는 [Spring Security Reference](http://docs.spring.io/spring-security/site/docs/3.2.5.RELEASE/reference/htmlsingle#jc-method) 에서 찾아볼 수 있다.

기본 ```AuthenticationManager```는 단독 사용자를 가진다('user' 사용자명과 난수 비밀번호가 애플리케이션을 시작하면 **INFO** 레벨로 출력된다).

```
Using default security password: 78fa095d-3f4c-48b1-ad50-e24c31d5cf35
```

제공되는 ```security.user.password``` 프로퍼티즈를 이용하여 비밀번호를 변경할 수 있다. 이것 외에 [SecurityProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/security/SecurityProperties.java) 의 다른 유용한 프로퍼티즈들로 확장가능하다(프로퍼티즈 접두어는 "security").

기본적인 보안 설정은 ```SecurityAutoConfiguration```의 구현체와 그 안에 임포트되어 있는 클래스들(웹보안을 위한 ```SpringBootWebSecurityConfiguration``` 과 비-웹 애플리케이션과 관련된 인증설정을 위한 ```AuthenticationManagerConfiguration```)이 있다. ```@EnableWebSecurity``` 와 빈을 추가하는 것으로 웹 애플리케이션의

## 28. <a name="SQL 데이터베이스 작업">SQL 데이터베이스 작업</a>
스프링 프레임워크는 SQL 데이터베이스에서 동작하는 넓은 지원을 제공한다. ```JdbcTemplate```를 사용하여 바로 JDBC에 접속하는 것부터 '객체 관계 매핑' 기술의 하이버네이트까지 폭넓게 지원한다. 스프링 데이터는 인터페이스로부터 바로 ```Repository``` 구현체를 생성하고 메서드명으로부터 쿼리를 생성하는 관례를 사용할 수 있는 수준의 추가적인 기능성을 제공한다.

### 28.1. 데이터베이스 설정<a name="데이터베이스 설정"></a>
자바의 ```javax.sql.DataSource``` 인터페이스는 데이터베이스 연결을 위한 표준 메서드를 제공한다. 기본적으로 데이터소스는 데이터베이스 연결을 생성하는 자격들을 얻는데 ```URL```을 사용한다.

#### 28.1.1. 내장형 데이터베이스 지원<a name="내장형 데이터베이스 지원"></a>
인-메모리 내장형 데이터베이스를 사용하면 애플리케이션을 개발하는데 편리하다. 당연히, 인-메모리 데이터베이스는 영속적인 저장소를 제공하지 않는다. 애플리케이션을 시작할 때와 애플리케이션을 종료할 때 데이터를 옮기기 위해 데이터베이스를 필요로 할 것이다.
> 팁: 어떻게 하는지는 [어떻게 데이터베이스를 초기화하는지 섹션](#데이터베이스 초기화)에 정리되어 있다.

스프링부트는 내장형 [H2](http://www.h2database.com/), [HSQL](http://hsqldb.org/)와 [Derby](http://db.apache.org/derby/) 데이터베이스를 자동설정할 수 있다. 특별히 연결 URL을 제공할 필요가 없다면, 사용하길 원하는 내장된 데이터베이스 의존성을 빌드에 포함시키면 된다.

예를 들어, 기본적인 POM 의존성은 다음과 같다:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
<dependency>
    <groupId>org.hsqldb</groupId>
    <artifactId>hsqldb</artifactId>
    <scope>runtime</scope>
</dependency>
```

> 노트: 자동설정을 위해 내장된 데이터베이스를 위한 ```spring-jdbc``` 의존성이 필요하다. ```spring-boot-starter-data-jpa``` 에 의해 자동으로 추가된다.

#### 28.1.2. <a name="외부 데이터베이스 연결">외부 데이터베이스 연결</a>
출시 데이터베이스 연결에는 ```DataSource```의 풀링 사용을 자동으로 설정할 수 있다. 여기 지정 구현체를 선택하는 알고리듬이 있다.
* 성능과 동시성을 위한 톰캣 풀링 ```DataSource``` 설정은, 언제든지 선택할 수 있다.
* HikariCP라면 사용가능하다.
* Commons DBCP라면 사용가지만, 출시 시에 사용하는 것은 권장하지 않는다.
* 마지막으로 Commons DBCP2는 사용가능하다.

만약 ```spring-boot-starter-jdbc```혹은 ``` spring-boot-starter-data-jpa``` 'starter POMs'를 사용한다면 자동적으로 ```tomcat-jdbc```에 관한 의존성이 자동으로 추가된다.
> 노트: 추가적인 커넥션 풀은 수동으로 설정해야 가능하다. 만약 ```DataSource``` 빈을 정의한다면, 자동설정은 동작하지 않는다.

데이터소스 설정은 외부 설정 프로퍼티즈의 ```spring.datasource.*```에 의해 조정된다. 예를 들어, 다음 섹션에서 다음과 같이 ```application.properties```를 정의할 것이다:
```
spring.datasource.url=jdbc:mysql://localhost/test
spring.datasource.username=dbuser
spring.datasource.password=dbpass
spring.datasource.driver-class-name=com.mysql.jdbc.Driver
```

[DataSourceProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jdbc/DataSourceProperties.java)를 보면 보다 자세한 제공옵션들을 확인할 수 있다.
> 팁: 굳이 driver-class-name 을 정의할 필요는 없다. 스프링부트는 url로 부터 대부분의 데이터베이스를 알아낼 수 있다.

> 노트: ```DataSource``` 풀링을 만들기 위해 ```Driver``` 클래스를 필요로 할수 있다, 그 때는 무언가를 하기 전에 체크를 한다. 예를 들어, ```spring.datasource.driverClassName=com.mysql.jdbc.Driver```를 설정하면 클래스는 적재가능해진다.

#### 28.1.3. <a name="JNDI 데이터베이스 연결">JNDI 데이터베이스 연결</a>
스프링부터 애플리케이션을 애플리케이션 서버에 배포하려할 때 데이터베이스에 대한 설정과 관리를 애플리케이션 빌트-인 기능들과 접근에 JNDI를 사용하고 싶을 수도 있다.

```spring.datasource.jndi-name``` 속성은 지정된 JNDI 위치에 ```DataSource```에 접근하기 위한 ```spring.datasource.url```, ```spring.datasource.username```과 ```spring.datasource.password``` 프로퍼티즈를 대신할 수 있다. 예를 들어, 다음과 같이 ```application.properties```를 보면 어떻게 ```DataSource```를 정의하여 JBoss AS에 접근할 수 있는지 알 수 있다.
```
spring.datasource.jndi-name=java:jboss/datasource/customers
```

### 28.2. <a name="JdbcTemplate 사용">JdbcTemplate 사용</a>
스프링의 ```JdbcTemplate``` 와 ```NamedParameterJdbcTemplate``` 클래스들은 자동설정되어 있으며 ```@Autowired```를 이용해서 빈에 바로 주입할 수 있다.
```
@Component
public class MyBean {

    private final JdbcTemplate jdbcTemplate;

    @Autowired
    public MyBean(JdbcTemplate jdbcTemplate) {
        this.jdbcTemplate = jdbcTemplate;
    }

    // ...

}
```

### 28.3. <a name="JPA 그리고 'Spring Data'">JPA 그리고 'Spring Data'</a>
자바 영속 API(Java Persistence API)는 객체와 데이터베이스의 관계를 연결하는 표준기술이다. ```spring-boot-stater-data-jpa``` POM이 빠르게 시작할 수 있는 방법을 제공한다. 주요 의존성은 다음과 같다.
* 하이버네이트Hibernate - JPA 구현체 중에서 많이 사용되고 있음
* Spring Data JPA -  JPA 기반의 저장소들을 쉽게 사용할 수 있도록 만들어줌
* Spring ORMs - 스프링 프레임워크에서 핵심 ORM을 지원함

> 팁: 여기서 JPA 혹은 Spring Data 에 대해서는 상세히 다루지는 않는다. [spring.io](http://spring.io/)에서 [JPA로 데이터에 접근하기'Accessing Data with JPA'](http://spring.io/guides/gs/accessing-data-jpa/)와 [Spring Data JPA](http://projects.spring.io/spring-data-jpa/)와 [Hibernate](http://hibernate.org/orm/documentation/) 참고문서를 살펴보기 바란다.

#### 28.3.1. <a name="엔티티 클래스">엔티티 클래스</a>
JPA 'Entity' 클래스는 ```persistence.xml``` 파일에 정의한다. 스프링부트는 이 파일을 필요로 하지 않으며 대신에 'Entity Scanning'을 사용한다. 기본적으로 메인설정클래스(```@EnableAutoConfiguration```  혹은 ```@SpringBootApplication``` 어노테이션이 있는 클래스)가 있는 패키지를 기준으로 모든 패키지를 검색한다.

```@Entity```, ```@Embeddable``` 혹은 ```@MappedSuperClass``` 어노테이드된 클래스들이 대상이 된다. 일반적인 엔티티 클래스는 다음과 유사한 모습을 가진다.

```java
package com.example.myapp.domain;

import java.io.Serializable;
import javax.persistence.*;

@Entity
public class City implements Serializable {

    @Id
    @GeneratedValue
    private Long id;

    @Column(nullable = false)
    private String name;

    @Column(nullable = false)
    private String state;

    // ... additional members, often include @OneToMany mappings

    protected City() {
        // no-args constructor required by JPA spec
        // this one is protected since it shouldn't be used directly
    }

    public City(String name, String state) {
        this.name = name;
        this.country = country;
    }

    public String getName() {
        return this.name;
    }

    public String getState() {
        return this.state;
    }

    // ... etc

}
```

> 팁: ```@EntityScan``` 어노테이션을 사용하면 엔티티 스캔위치를 변경할 수 있다. 이와 관련된 내용은 [섹션 68.4. 스프링 설정으로 부터 @Entity 정의 분리](#스프링 설정으로 부터 @Entity 정의 분리)를 보면 어떻게 하는지 알 수 있을 것이다.

#### 28.3.2. <a name="Spring Data JPA 레파지토리">Spring Data JPA 레파지토리</a>
Spring Data JPA 레파지토리는 데이터에 대한 접근을 정의할 수 있는 인터페이스들이다. JPA 쿼리는 메서드의 이름으로부터 자동으로 쿼리를 생성한다. 예를 들어, ```CityRepository``` 인터페이스에 ```findAllByState(String state)``` 메서드가 정의되어 있다면 state를 주고 모든 도시를 검색할 것이다.

보다 복잡한 쿼리는 Spring Data의 [Query](http://docs.spring.io/spring-data/jpa/docs/current/api/org/springframework/data/jpa/repository/Query.html) 어노테이션을 메서드에 어노테이드하여 사용할 수 있다.

스프링 데이터 레파지토리는 [```Repository```](http://docs.spring.io/spring-data/commons/docs/current/api/org/springframework/data/repository/Repository.html) 혹은 [```CrudRepository```](http://docs.spring.io/spring-data/commons/docs/current/api/org/springframework/data/repository/CrudRepository.html)를 확장한다. 만약에 자동설정을 사용한다면, 레파지토리는 (```@EnableAutoConfiguration``` 혹은 ```@SpringBootApplication``` 중 하나가 선언되어 있는)메인설정클래스가 있는 패키지부터 아래로 검색을 할 것이다.

여기 전형적인 스프링 데이터 레파지토리가 있다:
```
package com.example.myapp.domain;

import org.springframework.data.domain.*;
import org.springframework.data.repository.*;

public interface CityRepository extends Repository<City, Long> {

    Page<City> findAll(Pageable pageable);

    City findByNameAndCountryAllIgnoringCase(String name, String country);

}
```

> 팁: 우리는 Spring Data JPA의 표면을 거의 긁어냈다.<작가주>이 표현은... 모르겠음. @_@)</작가주> 보다 자세한 내용은 [참조 문서](http://projects.spring.io/spring-data-jpa/)를 확인하라.

#### 28.3.3. <a name="JPA 데이터베이스 생성 및 삭제">JPA 데이터베이스 생성 및 삭제</a>
기본적으로, JPA  데이터베이스는 내장된 데이터베이스(H2, HSQL 혹은 Derby)를 사용할 경우 자동적으로 생성된다. ```spring.jpa.*``` 프로퍼티즈를 사용한 JPA  설정을 통해 보다 명확하게 설정할 수 있다. 예를 들어, 테이블을 생성하고 제거하려면 다음과 같이 ```application.properties```에 추가할 수 있다.

```
spring.jpa.hibernate.ddl-auto=create-drop
```

> 노트: 이에 해당하는 하이버네이트의 내부 속성명은 ```hibernate.hbm2ddl.auto```이다(어떤 일이 벌어지는 지 기억하면 보다 이롭다). ```spring.jpa.properties.*```(접두사는 엔티티 매니저에 추가되기 전에 제거된다)를 사용하여 하이버네이트의 기존 프로퍼티즈를 설정할 수 있다. 예:

```
spring.jpa.properties.hibernate.globally_quoted_identifiers=true
```

하이버네이트 엔티티 매니저에 ```hibernate.globally_quoted_identifiers```가 전달된다.

```ApplicationContext```가 시작할 때까지 기본적으로 DDL 실행(혹은 유효성 검사)은 지연된다. 하이버네이트 자동설정이 활성화되어 있다면 ```spring.jpa.generate-ddl``` 플래그를 사용하지 않는데 왜냐하면 ddl-auto 설정의 우선순위가 낮기 때문이다.

## 29. NoSQL 기술 작업<a name="NoSQL 기술 작업"></a>
스프링 데이터는 [MongoDB](http://projects.spring.io/spring-data-mongodb/), [Neo4J](http://projects.spring.io/spring-data-neo4j/), [Elasticsearch](https://github.com/spring-projects/spring-data-elasticsearch/), [Solr](http://projects.spring.io/spring-data-solr/), [Redis](http://projects.spring.io/spring-data-redis/), [Gemfire](http://projects.spring.io/spring-data-gemfire/), [Couchbase](http://projects.spring.io/spring-data-couchbase/) 그리고 [Cassandra](http://projects.spring.io/spring-data-cassandra/) 등을 포함한 다양한 NoSQL 기술에 접근할 수 있도록 돕는 프로젝트들을 추가할 수 있다.
스프링부트는 Redis, MongoDB, Elasticsearch, Solr 그리고 Gemfire 를 위한 자동설정을 지원한다. 다른 프로젝트들을 사용할 수도 있지만 필요하다면 설정을 변경할 수도 있다. [projects.spring.io/spring-data](http://projects.spring.io/spring-data)에 나와있는 참조문서들을 살펴보기 바란다.

### 29.1. 레디스Redis<a name="레디스Redis"></a>
[Redis](http://redis.io/)는 캐시, 메시지 브로커 그리고 풍부한 기능을 가진 key-value 를 저장한다. 스프링부트는 [jedis](https://github.com/xetorthio/jedis/)와 [Spring Data Redis](https://github.com/spring-projects/spring-data-redis)에서 제공하는 추상화된 기초적인 자동설정을 제공한다. ```spring-boot-starter-redis```을 'Starter POM'을 이용하면 손쉽게 의존성을 추가할 수 있다.

#### 29.1.1. 레디스 연결<a name="레디스 연결"></a>
다른 스프링 빈들에 자동설정된 ```RedisConnectionFactory```, ```StringRedisTemplate``` 혹은 vanilla ```RedisTemplate``` 인스턴스를 주입할 수 있다. 기본적으로 인스턴스들은 ```localhost:6379```를 사용하여 Redis 서버에 연결한다.
```java
@Component
public class MyBean {

    private StringRedisTemplate template;

    @Autowired
    public MyBean(StringRedisTemplate template) {
        this.template = template;
    }

    // ...

}
```

자동구성된 형태의 ```@Bean```을 추가할 경우 기본값을 대체할 것이다(```RedisTemplate```의 경우를 제외하고 그것의 타입이 아니라 'redisTemplate' 이름에 기초하여 제외한다). 만약 ```commons-pool2```이 클래스패스에 있다면 기본적으로 pooled 커넥션 팩토리를 가지게 될 것이다.

### 29.2. 몽고DB MongoDB<a name="몽고DBMongoDB"></a>
[몽고DB](http://www.mongodb.com/)는 전통적인 테이블 기반의 관계형 데이터를 대신하여 JSON과 유사한 구조를 가진 오픈소스 NoSQL 문서 데이터베이스다. 스프링부트는 ```spring-boot-starter-data-mongodb``` 'Starter POM'을 추가하면 몽고DB에서 동작하는 다양한 편의를 제공한다.

#### 29.2.1. 몽고DB 연결<a name="몽고DB 연결"></a>
스프링 빈에 자동설정된 ```com.mongodb.Mongo``` 인스턴스를 주입할 수 있다. 기본적으로 인스턴스는 몽고DB 서버에서 사용하는 URL ```mongodb://localhost/test``` 으로 연결될 것이다:

```java
import com.mongodb.Mongo;

@Component
public class MyBean {

    private final Mongo mongo;

    @Autowired
    public MyBean(Mongo mongo) {
        this.mongo = mongo;
    }

    // ...

}
```

```spring.data.mongodb.uri``` 속성을 설정하여 ```url```을 변경하거나 ```host/port```를 정의할 수도 있다. 예를 들어, ```application.properties```에 다음과 같이 정의할 수 있다:
```
spring.data.mongodb.host=mongoserver
spring.data.mongodb.port=27017
```

> 팁: ```spring.data.mongodb.port```를 정의하지 않으면 ```27017```을 기본으로 사용한다. 간단히 위의 예제에서 이 라인을 삭제하면 된다.

MongoDB의 연결 설정을 완전히 제어하려는 경우, 별도의 ```Mongo @Bean```을 선언하면 된다.

#### 29.2.2. ```MongoTemplate```<a name="MongoTemplate"></a>
스프링 데이터 몽고는 스프링의 ```JdbcTemplate```와 유사하게 설계된 [MongoTemplate](http://docs.spring.io/spring-data/mongodb/docs/current/api/org/springframework/data/mongodb/core/MongoTemplate.html) 클래스를 제공한다. 스프링부트의 자동설정된 ```JdbcTemplate``` 빈처럼 간단하게 주입할 수 있다.

```java
@Component
public class MyBean {

    private final MongoTemplate mongoTemplate;

    @Autowired
    public MyBean(MongoTemplate mongoTemplate) {
        this.mongoTemplate = mongoTemplate;
    }

    // ...

}
```

보다 자세한 내용은 ```MongoOperations``` Javadoc을 살펴보자.

#### 29.2.3. <a name="Spring Data 몽고DB 레파지토리">Spring Data 몽고DB 레파지토리</a>
스프링 데이터는 MongoDB를 지원하는 레파지토리를 포함하고 있다. 앞서 거론했던 JPA 레파지토리처럼, 메서드 네임을 바탕으로 하여 자동적으로 쿼리를 생성하는 기본 처리방식을 가지고 있다.

사실, 스프링 데이터 JPA와 스프링 데이터 MongoDB는 같은 공통 인프라스트럭처를 공유한다. 그래서 앞에서 다른 JPA 예제를, ```City```는 JPA ```@Entity```에서 몽고 데이터 클래스가 되었다, 동작 방식은 같다:
```java
package com.example.myapp.domain;

import org.springframework.data.domain.*;
import org.springframework.data.repository.*;

public interface CityRepository extends Repository<City, Long> {

    Page<City> findAll(Pageable pageable);

    City findByNameAndCountryAllIgnoringCase(String name, String country);

}
```

>팁:
스프링 데이터 MongoDB에 관해 보다 자세히 살펴보려면, 리치 객체 매핑기술을 포함하여, [참고문서](http://projects.spring.io/spring-data-mongodb/)를 살펴보기 바란다.

### 29.3. <a name="Gemfire">Gemfire</a>
[Spring Data Gemfire](https://github.com/spring-projects/spring-data-gemfire)는 [Pivotal Gemfire](http://www.gopivotal.com/big-data/pivotal-gemfire#details) 데이터 관리 플랫픔 접근하기 편리한 스프링에 친화적인 도구들을 제공한다. 편리하게 사용하기 위해서는 ```spring-boot-starter-data-gemfire``` 'Starter POM' 의존성을 추가해야한다. 현재는 Gemfire를 위한 자동설정을 제공하지는 않지만, [@EnableGemfireRepositories](https://github.com/spring-projects/spring-data-gemfire/blob/master/src/main/java/org/springframework/data/gemfire/repository/config/EnableGemfireRepositories.java) 애노테이션만 사용하면 스프링 데이터 레파지토리를 활성화할 수 있다.

### 29.4. <a name="Solr">Solr</a>
[Apache Solr](http://lucene.apache.org/solr/)는 검색엔진이다. 스프링부트는 [Spring Data Solr](https://github.com/spring-projects/spring-data-solr)에서 제공하는 solr 클라이언트 라이브러리와 추상화 되어 있는 기본적인 자동설정을 제공한다. ```spring-boot-starter-data-solr``` 'Starter POM' 의존성만 추가하면 쉽게 사용할 수 있다.

#### 29.4.1. <a name="Solr 연결">Solr 연결</a>
자동설정된 ```SolrServer``` 인스턴스를 다른 스프링 빈에 주입할 수 있다. 서버에 대한 기본적인 연결설정은 ```localhost:8993/solr```을 사용한다.

```
@Component
public class MyBean {

    private SolrServer solr;

    @Autowired
    public MyBean(SolrServer solr) {
        this.solr = solr;
    }

    // ...

}
```

만약에 ```SolrServer``` 타입의 ```@Bean```을 추가하면 그 빈으로 대체된다.

#### 29.4.2. <a name="Spring Data Elasticsearch 레파지토리">Spring Data Elasticsearch 레파지토리</a>
스프링 데이터는 Apache Solr을 위한 레파지토리 지원을 포함하고 있다. 앞서 거론했던 JPA 레파지토리처럼, 메서드 네임을 바탕으로 하여 자동적으로 쿼리를 생성하는 기본 처리방식을 가지고 있다.

사실, Spring Data JPA와 Spring Data Solr은 같은 공통 인프라스트럭처를 공유하고 있다. 그래서 앞서 다룬 JPA 예제에서 ```City```는 JPA ```@Entity```에서 ```SolrDocument``` 클래스가 되었다. 동작 방식은 같다.

> 팁
Spring Data Solr에 대한 보다 자세한 내용은 [참고문서]http://projects.spring.io/spring-data-solr/)를 살펴보기 바란다.

### 29.5. Elasticsearch<a name="Elasticsearch"></a>
[엘라스틱서치 Elastic Search](http://www.elasticsearch.org/)는 오픈소스, 분산, 실시간 검색 및 분석 엔진이다. 스프링 부트는 엘라스틱서치를 위한 기본적인 자동설정과 [Spring Data Elasticsearch](https://github.com/spring-projects/spring-data-elasticsearch)이 제공하는 추상화를 제공한다. ```spring-boot-starter-data-elasticsearch``` 'Starter POM'을 추가하면 의존성을 손쉽게 추가할 수 있다.

#### 29.5.1. Elasticsearch 연결<a name="Elasticsearch 연결"></a>
자동설정된 ```ElasticsearchTemplate``` 이나 엘라스틱서치 ```Client``` 인스턴스를 다른 스프링빈에 주입할 수 있다. 기본적인 인스턴스는 로컬 인메모리 서버에 접속된다(엘라스틱서치 텀즈 안에 ```NodeClient``` ), 그러나 ```spring.data.elasticsearch.clusterNodes``` 에 콤마로 구분된 'host:port' 목록을 설정하면 원격지 서버로 변경할 수 있다.
```java
@Component
public class MyBean {

    private ElasticsearchTemplate template;

    @Autowired
    public MyBean(ElasticsearchTemplate template) {
        this.template = template;
    }

    // ...

}
```

```ElasticsearchTemplate``` 타입의 ```@Bean```을 추가하면 기본을 대체하게 된다.

#### 29.5.2. 스프링 데이터 Elasticsearch 레파지토리<a name="스프링 데이터 Elasticsearch 레파지토리"></a>
스프링 데이터는 엘라스틱서치 지원을 위한 레파지토리를 포함한다. 앞서 살펴봤던 JPA 레파지터리처럼, 기본적인 쿼리 생성박식은 메서드명을 기반으로 하여 자동생성한다.

사실, Spring Data JPA 와 Spring Data Elasticsearch 는 공통 인프라스트럭처를 공유한다, 그래서 JPA에서 예제로 사용했던 ```City```를 ```@Entity``` 대신 엘라스틱서치 ```@Document``` 클래스로 대체하면 된다, 같은 방법으로 동작한다.

> 팁: Spring Data Elasticsearch에 대한 보다 자세한 사항은, [참고문서](http://docs.spring.io/spring-data/elasticsearch/docs/)를 살펴보기 바란다.

## 30. 메시징<a name="메시징"></a>
스프링 프레임워크는 메시징 시스템 통합을 위한 광버무이한 지원을 제공한다; 간단하게는 ```JmsTemplate```를 이용하여 JMS API를 간단하게 이요할 수 있는 것부터 비동기적으로 메시지를 수신하는 인프라스트럭처를 완성할 수 있다. 스프링 AMQP 는 'Advanced Message Queuing Protocol' 과 유사한 기능셋을 제공하고 부트는 ```RabbitTemplate``` 와 RabbitMQ를 위한 자동설정 옵션을 제공한다. 또한 스프링 웹소켓에서 기본적으로 STOMP 메시징을 지원하며 스프링부트는 starter와 자동설정을 제공한다(스프링 프레임워크 참고문서의 [적절한 섹션](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#jms)을 살펴보라). 스프링부트는 메시지 송수신을 위해 필요한 인프라를 자동구성한다.

### 30.1. JMS<a name="JMS"></a>
```javax.jms.ConnectionFactory``` 인터페이스는 JMS 브로커와 상호작용을 위한 ```javax.jms.Connection``` 를 만들기 위한 표준 메서드를 제공한다. 스프링이 JMS으로 동작하기 위해서는 ```ConnectionFactory```가 필요한데, 바로 생성할 필요없이 대신 더 높은 수준의 메시징 추상화에 의존할 수 있다.

#### 30.1.1. HornetQ 지원<a name="HornetQ 지원"></a>
스프링부트는 클래스패스 상에서 HornetQ가 탐색되었을 때 ```ConnectionFactory```를 자동설정할 수 있다. 만약 브로커broker가 존재한다면, 자동설정된 내장된 브로커가 구동된다(모드 속성이 명시적으로 설정되어 있지 않은 경우). 지원되는 모드는 ```embedded```(내장된 브로커는 명시적으로 필요하며 클래스패스 상에서 찾을 수 없는 경우 에러가 발생한다), 그리고 ```native```는 ```netty``` 전송 프로토콜을 사용하여 브로커에 연결한다. 레터가 설정되어 있다면, 스프링부트는 ```ConnectionFactory```를 설정하여 기본설정에 따라 로컬 머신에서 실행되고 있는 브로커에 연결한다.

> 노트:
```spring-boot-starter-hornetq```를 사용하면 기존에 존재하는 HornetQ 인스턴스 연결에 필요한 의존성 뿐만 아니라 스프링 인프라스트럭처는 JMS 와 통합이 가능해진다. ```org.hornetq:hornetq-jms-server``` 을 애플리케이션에 추가하고 내장 모드를 사용하면 된다.

HornetQ 설정은 ```spring.hornetq.*``` 확장 설정 속성에 의해 제어된다. 예를 들어, ```application.properties``` 에 다음과 같이 정의를 한다면:

```
spring.hornetq.mode=native
spring.hornetq.host=192.168.1.210
spring.hornetq.port=9876
```

내장된 브로커라면, 영속화 활성을 선택한다면, 목적지 목록을 만드는 것이 가능하다. 콤마로 구분된 목록을 정의하여 기본옵션의 브로커들을 생성한다; ```org.hornetq.jms.server.config.JMSQueueConfiguration``` 혹은 ``` org.hornetq.jms.server.config.TopicConfiguration``` 타입의 나은 큐와 토픽에 관한 설정을 빈으로 정의한다

지원사항에 대한 자세한 내용은 [HornetQProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jms/hornetq/HornetQProperties.java)를 살펴보기 바란다.

JNDI 룩럽은 전혀 관여하지 않으며 목적지(destination)는 HornetQ 구성에서 '이름' 속성 또는 구성을 통해 제공되는 이름을 사용하거나, 자신의 이름을 통해 해결한다.

#### 30.1.2. ActiveMQ 지원<a name="ActiveMQ 지원"><a/>
스프링부트는 클래스패스 상에서 ActiveMQ가 탐색되었을 때 ```ConnectionFactory```를 자동설정할 수 있다. 만약 브로커broker가 존재한다면, 자동설정된 내장 브로커가 구동된다(어떤 브로커 URL도 지정된 설정이 없다면).

ActiveMQ 설정은 ```spring.activemq.*``` 확장 설정 프로퍼티즈를 토해서 제어할 수 있다. 예를 들어, ```application.properties``` 에 다음과 같이 설정하면:
```
spring.activemq.broker-url=tcp://192.168.1.210:9876
spring.activemq.user=admin
spring.activemq.password=secret
```

설정과 관련된 지원사항을 보다 자세히 살펴보려면 [ActiveMQProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jms/activemq/ActiveMQProperties.java)를 살펴보기 바란다.

기본적으로, ActiveMQ는 목적지가 정의해야하는데 목적지가 정의되지 않았다면, 목적지는 제공된 이름을 기준으로 처리된다.

#### 30.1.3. JNDI ```ConnectionFactory``` 사용
애플리케이션 서버에서 스프링부트 애플리케이션을 실행하고 있는 경우 JMS ```ConnectionFactory```를 사용하여 JNDI를 검색한다. 기본위치인 ```java:/JmsXA``` 와 ```java:/XAConnectionFactory```를 점검할 것이다. 위치를 변경해야할 경우가 있다면 ```spring.jms.jndi-name``` 속성을 사용하면 된다.

```
spring.jms.jndi-name=java:/MyConnectionFactory
```

#### 30.1.4. 메시지 전송<a name="메시지 전송"></a>
스프링의 ```JmsTemplate```는 자동설정되며 다음과 같이 빈에 직접 autowired 할 수 있다.
```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.jms.core.JmsTemplate;
import org.springframework.stereotype.Component;

@Component
public class MyBean {

    private final JmsTemplate jmsTemplate;

    @Autowired
    public MyBean(JmsTemplate jmsTemplate) {
        this.jmsTemplate = jmsTemplate;
    }

    // ...

}
```

> 노트:
[JmsMessagingTemplate](http://docs.spring.io/spring/docs/4.1.3.RELEASE/javadoc-api/org/springframework/jms/core/JmsMessagingTemplate.html)(스프링 4.1에 추가)는 비슷한 방법으로 주입가능하다.

#### 30.1.5. 메시지 수신<a name="메시지 수신"></a>
JMS 인프라스트럭처가 존재한다면, ```@JmsListener```를 통해 리스너 엔드포인트를 정의할 수 있다. ```JmsListenerContainerFactory``` 가 정의된 것이 없다면, 자동적으로 1개가 설정된다.

```someQueue``` 목적지를 리스너 엔드포인트로 하는 컴포넌트를 생성해보자.

```java
@Component
public class MyBean {

    @JmsListener(destination = "someQueue")
    public void processMessage(String content) { ... }

}
```

보다 자세한 항목은 [EnableJms](http://docs.spring.io/spring/docs/4.1.3.RELEASE/javadoc-api/org/springframework/jms/annotation/EnableJms.html) Javadoc을 확인하자.

## 31. <a name="이메일 전송">이메일 전송</a>
스프링 프레임워크는 ```JavaMailSender``` 인터페이스를 이용하여 메일발송을 쉽게 추상화할 수 있는 기능을 제공하고 스프링부트는 스타터 모듈을 통해 쉬운 자동설정을 제공한다.
> 팁: 어떻게 ```JavaMailSender```를 사용하는지 자세한 내용을 알고 싶다면 [참조 문서](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#mail)를 클릭해보자.

만약 ```spring.mail.host``` 그리고 관련된 라이브러리들(```spring-boot-starter-mail```에 기본설정된)은 가능하다면, ```JavaMailSender```가 존재하지 않는다면 그것을 만들것이다. 센더는 ```spring.mail``` 네임스페이스를 통해 설정변경이 가능하니, 보다 자세한 부분들은 [MailProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/mail/MailProperties.java)를 살펴보자.

## 32. JTA를 이용한 트랜잭션 분산
스프리부트는 [Atomkos](http://www.atomikos.com/) 혹은 [Bitronix](http://docs.codehaus.org/display/BTM/Home) 등의 내장된 트랜잭션 매니저를 사용하여 다양한 XA 자원에 대응하는 분산 JTA 트랜잭션을 지원한다. JTA 트랜잭션은 안정적인 Java EE 애플리케이션 서버에 배포되었을 때 사용되기도 한다.

JTA 환경이 탐색되었을 떄, 스프링의 ```JtaTransactionManager```는 트랜잭션 관리를 시작한다. 자동설정된 JMS, DataSource 그리고 JPA 빈은 XA 트랜잭션을 지원하도록 향상될 것이다. 스프링의 표준같은 ```@Transactional```을 통해 분산된 트랜잭션을 사용할 수 있다. 만약 JTA 환경을 로컬 트랜잭션에 대해서 사용하길 원한다면 ```spring.jta.enabled``` 속성을 ```false```로 설정하여 JTA 자동설정을 비활성화할 수 있다.

### 32.1. Atomikos 트랜잭션 매니저 사용
Atomikos 는 스프링부트 애플리케이션에 내장시킬 수 있는 인기있는 오픈소스 트랜잭션 관리자다. ```spring-boot-starter-jta-atomikos``` Starter POM을 사용하여 Atomikos 라이브러리들을 사용할 수 있다. 스프링부트는 Atomikos를 자동설정하고 ```depends-on``` 설정은 스프링빈을 위한 정확한 기동과 정지 순위를 제공한다.

기본적으로 Atomikos 트랜잭션 로그는 애플리케이션 홈디렉토리(애플리케이션 jar 파일이 위치한 디렉토리)에서 ```transaction-logs``` 폴더에 작성한다. ```application.properties``` 파일에 ```spring.jta.log-dir``` 속성을 저으이하여 디렉토리를 변경할 수 있다. ```spring.jta```으로 시작하는 속성들을 통해 Atomikos ```UserTransactionServiceIml```를 변경할 수 있다. 자세한 사항은 [AtomikosProperties](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/jta/atomikos/AtomikosProperties.html)을 살펴보기 바란다.

> 노트:
다중 트랜잭션 관리는 같은 리소스 매니저들을 제어할 수 있는 것이 확실해야 한다. 각각의 Atomikos 인스턴스는 유일한 ID로 설정되어야 한다. 이 기본 ID는 Atomikos가 실행되는 머신의 IP주소를 사용한다. 제품의 유일성이 불확실하다면, 각 애플리케이션의 인스턴스에 ```spring.jta.transaction-manager-id``` 속성으로 설정할 수 있다.

### 32.2. Bitronix 트랜잭션 매니저 사용
Bitronix 는 JTA 트랜잭션 매니저 구현체로 인기있는 오픈소스 중 하나다. ```spring-boot-starter-jta-bitronix``` Starter POM을 통해 프로젝트에 Bitronix의 의존성을 추가할 수 있다. Atomikos 와 마찬가지로, 스프링부트는 자동적으로 Bitronix를 설정하고 빈의 기동과 정지 순위에 따라 후속 조치를 취한다.

기본 Bitronix 트랜잭션 로그 파일(```part1.btm``` 과 ```part2.btm```)은 애플리케이션 홈 디렉토리에 ```transaction-logs``` 폴더에 작성한다. ```spring.jta.log-dir``` 속성을 통해서 디렉토리를 변경할 수 있다. ```spring.jta```로 시장하는 속성들은 ```bitronix.tm.Configuration``` 빈과 연결되니, 변경하는 것이 가능하다. 자세한 내용은 [Bitronix 문서](http://btm.codehaus.org/api/2.0.1/bitronix/tm/Configuration.html)
를 살펴보기 바란다.

> 노트:
다중 트랜잭션 관리는 같은 리소스 매니저들을 제어할 수 있는 것이 확실해야 한다. 각각의 Bitronix 인스턴스는 유일한 ID로 설정되어야 한다. 이 기본 ID는 Bitronix가 실행되는 머신의 IP주소를 사용한다. 제품의 유일성이 불확실하다면, 각 애플리케이션의 인스턴스에 ```spring.jta.transaction-manager-id``` 속성으로 설정할 수 있다.

### 32.3. Java EE 에서 관리하는 트랜잭션 매니저 사용
만약 스프링부트 애플리케이션을 ```war``` 혹은 ```ear``` 로 압축하고 Java EE 애플리케이션 서버에 배포한다면, 애플리케이션 서버에서 제공하는 트랜잭션 매니저를 사용할 수 있다. 스프링 부트는 공통 JNDI 위치를 탐색하여 트랜잭션 매니저를 자동설정하려고 할 것이다(```java:comp/UserTransaction```, ```java:comp/TransactionManager``` 등등). 애플리케이션 서버에서 제공하는 트랜잭션 서비스를 사용한다면, 모든 자원들에 대해서 서버에 의해 관리되며 JNDI 외부로 드러나길 바랄 것이다. 스프링부트는 JNDI 경로 ```java:/JmsXA``` 혹은 ```java:/XAConnectionFactory``` 에서 ```ConnectionFactory```를 찾아 JMS 자동설정을 제공할 것이며 [spring.datasource.jndi-name](#JNDI 데이터베이스 연결) 속성을 사용하여 ```DataSource```에 대한 설정할 수 있다.

### 32.4. XA 그리고 non-XA JMS 연결 혼합
JTA를 사용할 때 주 JMS ```ConnectionFactory``` 빈은 분산트랜잭션에서 XA를 사용할 것이다. non-XA ```ConnectionFactory```를 사용한 JMS 메시지 처리를 해야하는 경우가 있을 것이다. 예를 들어, JMS 처리 로직이 XA 타임아웃보다 긴 경우가 그렇다.

만약 non-XA ```ConnectionFactory```를 사용하려고 한다면 ```@Primary jmsConnectionFactory```보다 ```nonXaJmsConnectionFactory``` 빈을 주입하면 된다. ```jmsConnectionFactory``` 빈은 또한 또한 ```xaJmsConnectionFactory``` 빈 별칭을 제공한다.

예를 들어:
```bean
// Inject the primary (XA aware) ConnectionFactory
@Autowired
private ConnectionFactory defaultConnectionFactory;

// Inject the XA aware ConnectionFactory (uses the alias and injects the same as above)
@Autowired
@Qualifier("xaJmsConnectionFactory")
private ConnectionFactory xaConnectionFactory;

// Inject the non-XA aware ConnectionFactory
@Autowired
@Qualifier("nonXaJmsConnectionFactory")
private ConnectionFactory nonXaConnectionFactory;
```

### 32.5. 대안적인 내장형 트른잭션 매니저 지원
[XAConnectionFactoryWrapper](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/jta/XAConnectionFactoryWrapper.java)와 [XADataSourceWrapper](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/jta/XADataSourceWrapper.java) 인터페이스는 내장형 트른잭션 매니저들을 지원하는데 사용할 수 있다. 인터페이스는 ```XAConnectionFactory``` 그리고 ```XADataSource```빈을 감싸고 ```ConnectionFactory``` 그리고 ```DataSource``` 빈즈로 내보내어 분산 트랜잭션에 등록한다. DataSource와 JM 자동설정은 ```JtaTransactionManager```빈을 가지고 있는 한 JTA 변형체를 사용하며 ```ApplicationContext```에 등록되어 있는 XA wrapper를 사용한다.

[BitronixXAConnectionFactoryWrapper](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/jta/BitronixXAConnectionFactoryWrapper.java) and [BitronixXADataSourceWrapper](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/jta/BitronixXADataSourceWrapper.java)는 XA wrapper를 어떻게 사용하는지 좋은 예제를 제공한다.

## 33. 스프링 통합
스프링통합Spring Integration은 메시징 추상화와 HTTP, TCP 등의 전송수단 들을 제공한다. 만약 스프링통합을 클래스패스 상에서 사용하기 위해서는 ```@EnableIntegration``` 애노테이션을 이용하여 초기화한다. 'spring-integration-jmx'가 클래스패스에 있을 경우 메시징 프로세싱 분석은 JMX를 통해 제공될 것이다. 보다 자세한 사항은 [IntegrationAutoConfig](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/integration/IntegrationAutoConfiguration.java)를 살펴보자.

## 34. JMX를 통해서 모니터링과 관리
자바 관리 확장(Java Management Extension, JMX)는 모니터링과 애플리케이션 관리를 위한 표준 메카니즘을 제공한다. 스프링부트는 기본적으로 'mbeanServer' 라는 아이디를 가진 ```MBeanServer```의 빈과 스프링 JMX 애노테이션(```@ManagedResource```, ```@ManagedAttribute```, ```@ManagedOperation```)이 사용된 다른 빈들을 만들어낸다.

보다 자세한 내용은 [JmxAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jmx/JmxAutoConfiguration.java)을 살펴보자.

## 35. 테스팅<a name="테스팅"></a>
스프링 부트는 어플리케이션을 테스트 하는 데에 쓸모있는 도구를 여러 개 제공한다. ```spring-boot-starter-test``` POM 은 Spring Test, JUnit, Hamcrest 와 Mockito 의존성을 제공한다.(|패키지묶음을 쓸 수 있도록 의존성 정보를 제공한다.) 그리고 ```org.springframework.boot.test``` 패키지 아래에 있는 핵심```spring-boot``` 모듈에는 유용한 테스트 유틸리티들이 있다.

## 35.1. 테스트 스코프 의존성
'시작 POM'(```test scope```에서)(+으로) ```spring-boot-starter-test``` 를 사용한다면 아래처럼 제공되는 라이브러리를 볼 수 있을 것이다.

 - Spring Test — 스프링 어플리케이션을 위한 통합 테스트
 - JUnit — Java 어플리케이션을 유닛테스트 할 때 (+거의) 표준
 - Hamcrest — JUnit assertion(|단언) 스타일을 따르는 매처 오브젝트(서술부 혹은 한정사로 알려져있다)
 - Mockito — 자바 Mock 프레임워크

이 (+라이브러리)들은 테스트를 작성할 때 유용하게 쓰이는 공통 라이브러리다. 이 라이브러리들이 적당하지 않다고 생각한다면 자유롭게 다른 테스트 (라이브러리)의존성을 추가할 수 있다.

### 35.2. 스프링 애플리케이션 테스트
의존성 주입으로 얻는 가장 큰 장점 하나는 작성한 코드가 유닛테스트 하기 쉬워진다는 것이다. 심지어 스프링과 조금도 상관없이, ```new``` 명령을 사용해서 오브젝트를 간단하게 인스턴스화 할 수 있다. 그리고 *목 객체[mock objects]*를 실제 의존하는 대상 대신 사용할 수도 있다.

종종 '유닛 테스팅'을 마치고 '통합 테스팅'을 시작해야 한다(통합 테스팅 과정에 스프링 ```ApplicationContext```이 실제로 개입하게 된다). 이때 어플리케이션을 디플로이하거나 다른 기반 기술과 연결할 필요 없이 통합 테스트가 가능하도록 만드는 것이 좋다.

스프링 프레임워크는 딱 이런 통합 테스트 전용 테스트 모듈을 포함하고 있다. ```org.springframework:spring-test```에 대한 의존성을 직접 선언하거나 'Starter POM'에 ```spring-boot-starter-test```을 사용하여 (+메이븐이) 가져오도록 설정할 수 있다.

```spring-test``` 모듈을 써본 적이 없다면 스프링 프레임워크 레퍼런스에서 [관련부분](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#testing) 을 읽고 시작하는 것이 좋을 것이다.

### 35.3. 스프링부트 애플리케이션 테스트<a name="스프링부트 애플리케이션 테스트"></a>
스프링 부트 어플리케이션은 그냥 스프링 `ApplicationContext` 이므로 평범한[vanilla] 스프링 컨텍스트를 가지고 하려는 일 대부분은 테스트 할  때 특별히 해줘야 하는 것은 없다. 다만 한 가지 주의할 것은 `SpringApplication` 을 생성해서 사용한다면 로깅 등 스프링 부트의 기능, 외부 속성(|프로퍼티)은 컨텍스트에만 자동으로 설치해야한다는 것이다.(? 컨텍스트 안에 자동 설치되도록 해야만  `SpringApplication`을 쓸 수 있나?)

스프링 부트는 표준 ```spring-test``` ```@ContextConfiguration``` 어노테이션 대신에 ```@SpringApplicationConfiguration``` 어노테이션을 제공한다. 테스트에 사용하는 ```ApplicationContext```를 설정할 때 ```@SpringApplicationConfiguration``` 를 사용하면 ```SpringApplication```에 의해 (+```ApplicationContext```가) 생성되고 스프링 부트의 추가 기능을 쓸 수 있을 것이다.
예를 보자 :
```java
@RunWith(SpringJUnit4ClassRunner.class)
@SpringApplicationConfiguration(classes = SampleDataJpaApplication.class)
public class CityRepositoryIntegrationTests {

    @Autowired
    CityRepository repository;

    // ...

}
```

컨텍스트 로더는 ```@WebAppConfiguration``` 어노테이션을 찾아서 웹 어플리케이션을 테스트 할 것인지 아닌지(예를 들어 ```MockMVC```를 사용한다든지) 추측한다. (```MockMVC``` 와 ```@WebAppConfiguration``` 은 ```spring-test```의 일부분이다).

(+테스트할 때 실제로) 웹 어플리케이션을 시작하고 포트에서 수신(|대기)하게 하려면  테스트할 클래스(또는 테스트할 클래스의 슈퍼 클래스 중 하나)에 ```@IntegrationTest``` 을 표시하여 HTTP(예를 들면 ```RestTemplate```을 사용하고) 를 써서 테스트 할 수 있다. 이 (+```@IntegrationTest```)는 매우 유용한데, 어플리케이션을 풀 스택으로 테스트할 수 있을 뿐만 아니라 컴포넌트들을 테스트 클래스에 주입하고 HTTP 상호작용이 끝난 다음 내부 상태를 단정[assert]할 수 있기 때문이다. 예시 :
```java
@RunWith(SpringJUnit4ClassRunner.class)
@SpringApplicationConfiguration(classes = SampleDataJpaApplication.class)
@WebAppConfiguration
@IntegrationTest
public class CityRepositoryIntegrationTests {

    @Autowired
    CityRepository repository;

    RestTemplate restTemplate = new TestRestTemplate();

    // ... interact with the running server

}
```
> 스프링의 테스트 프레임워크는 각 테스트 사이에 어플리케이션 컨텍스트를 캐쉬해둔다(|보관한다). 그러므로 테스트들이 같은 설정을 공유하는 한 실제로 테스트를 몇 개나 실행하든 상관없이 서버를 시작하고 멈추는 과정에서 시간을 소모하는 일은 딱 한 번 일어난다.

포트를 바꾸고 싶다면 ```@IntegrationTest```에 환경 속성을 콜론(+;)이나 대입식 이름-값 묶음으로 추가하면 된다. 예를 들면  ```@IntegrationTest("server.port:9000")``` 와 같은 식이다. 게다가 ```server.port``` 와 ```management.port``` 속성을 `0`으로 설정하면 임의의 포트로 통합테스트 할 수있다. 예제 :
```java
@RunWith(SpringJUnit4ClassRunner.class)
@SpringApplicationConfiguration(classes = MyApplication.class)
@WebAppConfiguration
@IntegrationTest({"server.port=0", "management.port=0"})
public class SomeIntegrationTests {

    // ...

}
```
테스트를 실행하는 동안 실제로 할당된 포트를 알아내고 싶다면 [Section 64.4, “Discover the HTTP port at runtime”](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/reference/html/howto-embedded-servlet-containers.html#howto-discover-the-http-port-at-runtime) 문서를 보라.

#### 35.3.1. 스팍Spock을 사용하여 스프링 부트 애플리케이션 테스트
Spock 을 스프링 부트 어플리케이션을 테스트하는 데 사용하고 싶다면 Spock의 `spock-spring` 모듈에 대한 의존성을 어플리케이션 빌드에 추가해야한다. `spock-spring`은 스프링 테스트 프레임워크를 Spock 안에 포함하고 있다.

Spock은 `@ContextConfiguration` [메타 어노테이션](https://code.google.com/p/spock/issues/detail?id=349)을 [찾아내지 않으므로](https://code.google.com/p/spock/issues/detail?id=349) [위에서 설명한](#스프링부트 애플리케이션 테스트) `@SpringApplicationConfiguration` 을 사용할 수 없다는 것을 명심하라. 이런 제한을 피하려면 `@ContextConfiguration` 어노테이션을 직접 사용해서 스프링 부트가 명확한(|특정한) 컨텍스트 로더를 사용하도록 설정해야한다.
```java
@ContextConfiguration(loader = SpringApplicationContextLoader.class)
class ExampleSpec extends Specification {

	    // ...

}
```
> (+이렇게 하면) [위에서 설명한](#스프링부트 애플리케이션 테스트) 어노테이션은 Spock과 함께 사용할 수 있다. 즉 @IntegrationTest 와 @WebAppConfiguration 을 필요로 하는 테스트에 따라 (+위 예제의)`Specification` (+클래스)에 표시(|사용)할 수 있다.

### 35.4. 테스트 유틸리티<a name="테스트 유틸리티"></a>
`spring-boot` 에는 대부분의 어플리케이션을 테스트할 때 쓸모있는 테스트 유틸리티가 들어있다.

#### 35.4.1. ```ConfigFileApplicationContextInitializer```
`ConfigFileApplicationContextInitializer` 은 테스트에 스프링 부트 `application.properties`파일을 로드해서 적용하는 `ApplicationContextInitializer` 이다. `@SpringApplicationConfiguration`이 제공하는 모든 기능이 필요없을 때 사용한다.
```java
@ContextConfiguration(classes = Config.class,
    initializers = ConfigFileApplicationContextInitializer.class)
```
#### 35.4.2. ```EnvironmentTestUtils```
`EnvironmentTestUtils` 는 `ConfigurableEnvironment` 나 `ConfigurableApplicationContext` 에 속성을 빠르게 추가할 수 있도록 해준다. `key=value` 스트링으로 간단하게 호출할 수 있다:
```java
EnvironmentTestUtils.addEnvironment(env, "org=Spring", "name=Boot");
```

#### 35.4.3. ```OutputCapture```
`OutputCapture` 은 `System.out` 과 `System.err` 출력을 캡처하는 JUnit `Rule`이다. capture를 선언하고 `@Rule`을 표시하는 것으로 간편하게 단정문[assertion]에서 `toString()`을 사용할 수 있다.
```
import org.junit.Rule;
import org.junit.Test;
import org.springframework.boot.test.OutputCapture;

import static org.hamcrest.Matchers.*;
import static org.junit.Assert.*;

public class MyTest {

    @Rule
    public OutputCapture capture = new OutputCapture();

    @Test
    public void testName() throws Exception {
        System.out.println("Hello World!");
        assertThat(capture.toString(), containsString("World"));
    }

}
```

#### 35.4.4. ```TestRestTemplate```
`TestRestTemplate`은 스프링 `RestTemplate`의 편리한 서브 클래스로 통합 테스트를 할 때 유용하다. 평범한 템플릿을 사용하거나 기본 HTTP 인증(사용자 이름과 암호 사용)을 보내는 방법을 쓸 수 있다. 어느 경우든 템플릿이 테스트 친화적인 방법이 될 것이다 : 리다이렉트를 따라가지 않고(이러면 응답 위치를 단정(|테스트)할 수 있다), 쿠키를 무시하거나(템플릿은 이전 상태를 저장하지 않는 stateless이다), 서버 사이드 에러에 대해 예외를 던지지 않도록 한다
아파치 HTTP 클라이언트(4.3.2 또는 그 이상)을 사용하는 것은 추천이나 필수는 아니다. 클래스패스에 아파치 클라이언트가 있으면 `TestRestTemplate`는 클라이언트를 적당히 설정하여 응답할 것이다.

```java
public class MyTest {

    RestTemplate template = new TestRestTemplate();

    @Test
    public void testRequest() throws Exception {
        HttpHeaders headers = template.getForEntity("http://myhost.com", String.class).getHeaders();
        assertThat(headers.getLocation().toString(), containsString("myotherhost"));
    }

}
```
## 36. 자동설정으로 개발하고 @Condition 사용하기<a name="자동설정으로 개발하고 @Condition 사용하기"></a>
공유 라이브러리를 개발하는 회사에서 일하거나, 오픈소스 혹은 상용 라이브러리 회사에서 일한다면 고유한 자동설정을 만들고 싶을 것이다.
자동 설정 클래스는 외부 jar에 담길 수도 있고[can be bundled] 스프링 부트가 이것을 고르는 것도 가능하다.
### 36.1. 자동설정 빈 이해
내부(+구현)에선, 자동 설정은 표준 ```@Configuration``` 클래스를 가지고 구현되었다. 추가 ```@Conditional``` 어노테이션들은 자동 설정이 적용해야 할 때 제약으로 작용한다(|제약한다)
대개 자동 설정클래스들은 ```@ConditionalOnClass``` 와 ```@ConditionalOnMissingBean``` 어노테이션을 사용한다. 이(+어노테이션)는 자동 설정이 적절한 클래스가 발견되었을 때와 직접 선언한 ```@Configuration```이 없을 때에만 적용되는 것을 보장한다.
우리가 제공하는 ```@Configuration``` 클래스를 보려면 ```spring-boot-autoconfigure``` 의 소스 코드를 살펴보면 된다(```META-INF/spring.factories``` 파일을 보라).
### 36.2. 자동설정 위치 후보지(|후보 찾아내기)
스프링 부트는 배포한[published] jar 안에 ```META-INF/spring.factories``` 가 있는지 체크한다. 이 파일은 ```EnableAutoConfiguration``` 키 에 당신의 설정 클래스를 나열하고(|담고) 있어야 한다.

```properties
org.springframework.boot.autoconfigure.EnableAutoConfiguration=\
com.mycorp.libx.autoconfigure.LibXAutoConfiguration,\
com.mycorp.libx.autoconfigure.LibXWebAutoConfiguration
```

설정이 특정한 순서대로 적용되어야 한다면 ```@AutoConfigureAfter``` 나 ```@AutoConfigureBefore``` 어노테이션을 사용하면 된다. 예를 들어, 웹에 국한된 설정을 제공하려 한다면 당신의 설정 클래스는 ```WebMvcAutoConfiguration``` 다음에 적용되어야 할 수도 있다.

### 36.3. 컨디션 애노테이션 @Condition<a name="컨디션 애노테이션 @Condition"></a>
여러분은 대개 자동설정에 하나 혹은 그 이상 ```@Condition``` 어노테이션을 포함하기를 바란다(|바랄 것이다). ```@ConditionalOnMissingBean``` 은 개발자가 여러분의 기본(+설정)이 만족스럽지 않으면 자동설정을 'override'하도록 허용하는 것을 보여주는 예이다.

스프링 부트는 ```@Conditional``` 어노테이션을 여러 개 포함하고 있는데 이것은 여러분 코드에서 ```@Configuration``` 클래스나 각 ```@Bean``` 메소드를 표기함으로써 재사용할 수 있다.
(?```@Configuration``` 을 클래스 정의에 붙여주거나 ```@Bean을``` 메소드에 붙여준다는 의미인지?)

#### 36.3.1. 클래스 조건
```@ConditionalOnClass``` 와 ```@ConditionalOnMissingClass``` 어노테이션은 특정 클래스가 존재하거나 존재하지 않는 경우에 대해서 설정을 건너 뛸 수 있도록 해준다. 어노테이션 메타데이터는 [ASM](http://asm.ow2.org/) 을 이용하여 파싱되므로 실행중인 어플리케이션의 클래스패스에 해당 클래스가 나타나지 않더라도 실제 클래스를 참조하는 ```value``` 속성을 사용할 수 있다. ```String``` 값을 사용하여 클래스 이름을 명시하는 것을 선호한다면 ```name``` 속성을 사용할 수도 있다.

#### 36.3.2. 빈Bean 조건
```@ConditionalOnBean``` 과 ```@ConditionalOnMissingBean``` 어노테이션은 특정 빈이 존재하거나 존재하지 않는 경우에 대해서 설정을 건너뛸 수 있도록 해준다. 타입으로 특정 빈을 명시하는 데에 ```value``` 속성을 사용하거나 이름으로 명시할 때 ```name``` 속성을 사용할 수 있다. ```search``` 속성을 사용하여 빈을 찾을 때 ```ApplicationContext``` 계층에 제한을 둘 수 있다.

> ```@Conditional``` 어노테이션은 ```@Configuration``` 클래스들이 파싱될 때 (+함꼐) 처리된다. 자동설정 ```@Configuration``` 은 항상 나중에(사용자가 정의한어떠한 빈들 다음에) 파싱된다. 하지만 이 어노테이션(?```@Conditional```?) 을 보통 ```@Configuration``` 클래스에 사용하려 한다면 아직 생성하지 않은 빈의 정의를 참조하지 않도록 주의해야한다.

#### 36.3.3. 특성(|프로퍼티) 조건
```@ConditionalOnProperty```` 어노테이션은 스프링 환경 특성(|프로퍼티)에 따라 설정을 할 수 있도록 해준다. ```prefix``` 와 ```name``` 속성으로 체크해야할 특성을 명시한다. 존재하고 ```false```가 아닌 특성은 기본적으로(|설정 없이도|자동으로) 매치가 될 것이다. 상세하게 체크하고 싶다면 ```havingValue``` 와 ```matchIfMssing``` 속성을 사용하면 된다.

#### 36.3.4. 리소스 조건
```@ConditionalOnResource``` 어노테이션은 특정 리소스가 존재할 때에만 설정을 할 수 있도록 해준다. 리소스는 보통 스프링 관례를 따라 나타낼 수 있다. 예를 들어, 파일은 ```file:/home/user/test.dat``` 로 나타낼 수 있다.

#### 36.3.5. 웹 어플리케이션 조건
```@ConditionalOnWebApplication``` 과 ```@ConditionalOnNotWebApplication``` 어노테이션은 어플리케이션이 '웹 어플리케이션'인지 아닌지에 따라 설정을 건너뛸 수 있게 해준다. 스프링 ```WebApplicationContext``` 를 사용하고, ```session``` 스코프를 정의하거나 ```StandardServletEnvironment``` 를 가지고 있는 어플리케이션은 웹 어플리케이션으로 본다(|취급한다).

#### 36.3.6. SpEL 표현식 조건
```@ConditionalOnExpression``` 어노테이션은 [SpEL expression](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#expressions) 결과에 따라 설정을 건너뛸 수 있게 해준다.

## 37. 웹소켓
스프링부트는 내장형 톰캣(7과 8) 그리고 내장형 Jetty 9에 대한 웹소켓 자동설정을 제공한다. 만약 war 파일을 단독 컨테이너에 배포할 경우, 스프링부트는 컨테이너가 웹소켓을 지원하는 설정을 제공하는지 확인한다.

스프링 프레임워크는 [rich WebSocket support](http://docs.spring.io/spring/docs/4.1.3.RELEASE/spring-framework-reference/htmlsingle/#websocket)를 ```spring-boot-starter-websocket``` 모듈을 통해 쉽게 접근할 수 있도록 제공한다.

## 38. 다음 읽을거리
다른 항목들에 대한 보다 깊이 살펴보길 바란다면 [Spring Boot API 문서](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api)이나 [소스코드](http://github.com/spring-projects/spring-boot/tree/master)를 바로 살펴보길 바란다. 만약 특정된 궁금증을 가지고 있다면 ['어떻게How-to' 가이드](#'어떻게How-to' 가이드)를 살펴보기 바란다.

스프링부트의 핵심 기능들에 대해서 충분히 숙지했다면, [스프링부트 액츄에터: 출시준비 기능들](#스프링부트 액츄에터: 출시준비 기능들)으로 이동하도록 하자.

# V. 스프링부트 액츄에터: 출시준비 기능들<a name="스프링부트 액츄에터: 출시준비 기능들"></a>
스프링부트는 제품을 출시했을 때 애플리케이션을 관찰하고 관리하는데 유용한 많은 기능들을 포함하고 있다. HTTP endpoints, 그리고 JMX 혹은 리모트 쉘(SSH 혹은 Telnet) 등 다양한 기능 중에서 어떤 기능을 이용하여 애플리케이션을 관리하고 관찰할 지 결정할 수 있다. 애플리케이션에서 감시audting, 건강health 그리고 측정metrics 을 자동으로 획득할 수 있다.

## 39. 사용가능한 출시준비 기능들<a name="사용가능한 출시준비 기능들"></a>
[```spring-boot-actuator```](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator) 모듈은 스프링부트의 출시준비 기능을 제공한다. ``` spring-boot-starter-actuator``` 'Starter POM' 의존성을 추가하는 것만으로 간단하게 기능을 활서오하할 수 있다.

#### 액츄에이터 정의
액체에이터는 기간동안 생산하고, 무엇인가를 제어하거나 움직이기 위해 기계적인 장치를 참조하는 것이다. 액츄에이터는 작은 변화로부터 큰 변화를 만들어낼 수 있다.

메이븐 기반의 프로젝트에 액츄이에터를 추가하는, 'starter' 의존성을 추가해보자:
```xml
<dependencies>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-actuator</artifactId>
    </dependency>
</dependencies>
```

그레들에서는 다음과 같이 정의한다:
```
dependencies {
    compile("org.springframework.boot:spring-boot-starter-actuator")
}
```

## 40. 엔드포인트<a name="엔드포인트"></a>
액츄에이터 엔드포인트는 애플리케이션에 대한 감시와 상호작용을 허용한다. 스프링부트는 작성가능한 엔드포인트들을 포함하고 있으며 필요에 따라 추가할 수 있다. 예를들어 ```health``` 엔드포인트는 애플리케이션의 기본적인 건강정보를 제공한다.

엔드포인트는 선택하는 기술에 따라서 노출되는 방법이 달라진다. 대부분의 애플리케이션은 엔드포인트의 ID가 URL과 매핑된 HTTP 모니터링을 선택한다. 예를 들어, 기본적으로, ```health``` 엔드포인트는 ```/health```에 매핑된다.

사용가능한 엔드포인트는 다음과 같다.

| ID           | 설명                  | 민감도                |
|--------------|-----------------------|----------------------|
| ```autoconfig``` | '사용' 혹은 '비사용'된 모든 자동구성 후보와 이유를 보여주는 자동구성 보고서를 표시합니다. | true |
| ```beans``` | 애플리케이션에 등록된 스프링빈 목록을 보여준다.| true |
| ```configprops``` | 모든 ```@ConfigurationProperties```를 보여준다. | true |
| ```dump``` | thread dump 수행결과를 보여준다. | true |
| ```env``` | 스프링의 ```ConfigurableEnvironment``` 정보를 보여준다. | true |
| ```health``` | 애플리케이션의 건강상태 정보를 보여준다. 기본은 'OK' 만 | false |
| ```info``` | 임의적인 애플리케이션의 정보를 보여준다. | false |
| ```metrics``` | 현재 애플리케이션의 metrics를 보여준다. | true |
| ```mappings``` | 모든 ```@RequestMapping``` 경로를 보여준다. | true |
| ```shutdown``` | 애플리케이션을 정상적으로 종료한다(기본은 비활성화). | true |
| ```trace``` | Trace 정보를 보여준다(기본적으로는 최근의 HTTP 요청을 보여줌). | true |

> 노트:
엔드포인트를 어떻게 노출할지는 ```sensitive``` 파라미터에 따라 보안요소가 적용된다. 예를 들어, sensitive 엔드포인트는 HTTP 접근시 사용자명/비밀번호를 요구할 것이다(혹은 웹 시큐리티를 비활성화하면 간단히 비활성화된다).

### 40.1. 엔드포인트 변경<a name="엔드포인트 변경"></a>
엔트포인트는 스프링 프로퍼티즈를 사용하여 변경할 수 있다. 엔드포인트를 ```enabled```를 활성화로 변경한다면, ```sensitive```와 그 ```id```를 고려하자.

예를 들어, 여기 ```application.properties```는 ```beans``` 엔드포인트의 의 id와 sensitivity를 변경하고 ```shutdown```도 활성화 했다.

```
endpoints.beans.id=springbeans
endpoints.beans.sensitive=false
endpoints.shutdown.enabled=true
```
> 팁:
접미사 ```"endpoints + . + name"```엔드포인트의 유일한 식별자로 사용하고 한다.

### 40.2. 상태 정보 변경<a name="상태 정보 변경"></a>
```health``` 엔드포인트가 노출하는 기본정보는 간단하게 'OK' 메시지다. 이것은 건강상태를 점검하기 위한 용도로 자주 사용된다. 예를 들어, 데이터베이스 연결 혹은 원격지 REST endpoint 기능을 점검할 때 효과적이다.

[```HealthIndicator```](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/health/HealthIndicator.java) 인터페이스를 구현한 것을 스프링빈으로 등록하여 건강상태 정보를 변경하여 제공하는 것이 가능하다.

```java
import org.springframework.boot.actuate.health.HealthIndicator;
import org.springframework.stereotype.Component;

@Component
public class MyHealth implements HealthIndicator {

    @Override
    public Health health() {
        // perform some specific health check
        return ...
    }

}
```

스프링부트는 [```DataSourceHealthIndicator```](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/health/DataSourceHealthIndicator.java) 구현체는 Redis, MongoDB 그리고 RabbitMQ 등의 데이터베 베이스 점검(검증 쿼리가 있다면 그것을 재사용)을 실행한 정보를 제공한다. 스프링부트는 ```ApplicationContext``` 에 ```DataSource```, ```MongoTemplate```, ```RedisConnectionFactory``` 그리고  ```RabbitTemplate``` 타입의 빈이 있다면```HealthIndicator``` 인스턴스를 자동으로 구현한다. health indicator는 또한 디스크 빈 공간에 관한 정보를 제공한다.

```HealthIndicator``` 유형의 수정된 구현체는 ```Status``` 유형을 독창적으로 사용할 수 있다. 게다가 ```Status```를 동일하거나 보다 복잡한 시스템 상태를 표현하는 것도 가능하다.

이 경우 사용자가 정의한 ```HealthAggregator``` 인터페이스 구현체나 기본구현체는  필요한 정보들을  ```management.health.status.order``` 설정 속성을 사용해서 설정해야 한다.

```HealthIndicator``` 구현체 중 하나를 사용하여 새로운 ```Status```인 ```FATA```을 사용한다고 가정해보자. 애플리케이션의 속성 ```management.health.status.order: DOWN, OUT_OF_SERVICE, UNKNOWN, UP```을 따라 심각한 정도나 우선순위에 따라 추가한다.

### 40.3. 애플리케이션 정보 안내 변경
```info``` 엔드포인트는 스프링 속성 ```info.*``` 을 설정하여 노출되는 데이터를 변경할 수 있다. ```info``` 키 아래의 모든 ```Environment``` 속성들이 자동으로 노출된다. 예를 들어, ```application.properties``` 에 다음과 같이 추가해보자:

```
info.app.name=MyService
info.app.description=My awesome service
info.app.version=1.0.0
```

#### 40.3.1. 빌드 시간에 관한 속성 확장 자동화
하지만 프로젝트의 빌드구성에 지정된 일부 속성을 하드코딩하는 것보다, 자동으로 빌드 구성을 사용하여 info 속성들을 확장할 수 있습니다. Maven과 Gradle 모두 가능합니다.

#### 메이븐을 이용하여 속성 확장 자동화
메이븐 프로젝트는 리소스 필터링을 통해서 자동으로 info 속성을 확장한다. 만약 ```spring-boot-starter-parent``` 를 사용하고 있다면 메이븐 'project properties'들을 ```@..@``` placeholder로 참조할 수 있다.

```
project.artifactId=myproject
project.name=Demo
project.version=X.X.X.X
project.description=Demo project for info endpoint
info.build.artifact=${project.artifactId}
info.build.name=@project.name@
info.build.description=@project.description@
info.build.version=@project.version@
```

> 노트:
위의 예에서 리소스 메이븐 필터링이 어떤 이유로 변환되지 않은 경우 폴백으로서 사용될 일부값을 설정하는데 ```project.*```를 사용했다.

> 노트:
만약 starter parent를 사용하지 않는다면, ```pom.xml``` 에 ```<build/>``` 요소가 필요하다.

```xml
<resources>
    <resource>
        <directory>src/main/resources</directory>
        <filtering>true</filtering>
    </resource>
</resources>
```

and (inside ```<plugins/>```):

```xml
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-resources-plugin</artifactId>
    <version>2.6</version>
    <configuration>
        <delimiters>
            <delimiter>@</delimiter>
        </delimiters>
    </configuration>
</plugin>
```

#### 그레들을 이용하여 속성 확장 자동화
그레들 프로젝트는 Java 플러그인의 ```processResource``` 태스크로부터 info 속성들을 자동으로 설정한다.
```
processResources {
    expand(project.properties)
}
```

그레들 프로젝트의 속성들을 placeholder를 통해 참조할 수 있다.
```
info.build.name=${name}
info.build.description=${description}
info.build.version=${version}
```

#### 40.3.2. 깃 커밋 정보
한편으로 ```info``` 엔드포인트의 유용한 기능중 하나는 프로젝트가 빌드되었을 때 ```git``` 소스코드의 상태에 관한 정보를 노출할 수 있다. 만약 jar  파일에 있는 ```git.properties```  파일에 ```git.branch``` 그리고 ```git.commit``` 속성이 있다면 노출된다.

메이븐 사용자라면 ```spring-boot-starter-parent``` POM에 포함된 플러그인을 통해서 ```git.properties``` 파일을 생성할 수 있다. POM에 추가하는 방법은 간단하다:

```xml
<build>
    <plugins>
        <plugin>
            <groupId>pl.project13.maven</groupId>
            <artifactId>git-commit-id-plugin</artifactId>
        </plugin>
    </plugins>
</build>
```

그레들 사용자는 이와 유사한 [```gradle-git```](https://github.com/ajoberstar/gradle-git) 플러그인을 통해서 가능한데, 프로퍼티즈 파일을 생성하기 위해서는 약간의 추가적인 작업이 필요하다.

## 41. HTTP를 통해서 모니터링 및 관리<a name="HTTP를 통해서 모니터링 및 관리"></a>
스프링 MVC 애플리케이션을 개발하고 있다면, 스프링부트 액츄에이터는 HTTP를 통해서 모든 non-sensitive 엔드포인트 노출을 자동설정할 것이다. 기본적인 컨벤션은 ```id```를 URL 경로에 맞춰준다. 예를 들어 ```health```는 ```/health```로 노출된다.

### 41.1. 세밀한 엔드포인트 노출<a name="세밀한 엔드포인트 노출"></a>
만약 'Spring Security' sensitive 엔드포인트를 사용한다면 HTTP로 노출되기는 하지만, 보호가 된다. 기본적은 '기초' 인증은 사용자명으로 ```user```를 사용하고 비밀번호를 생성한다(애플리케이션이 시작하는 단계에서 출력된다).
> 팁:
생서된 비밀번호는 애플리케이션이 시작될 때 기록된다. 'Using default security password'로 검색한다.

스프링 프로퍼티즈를 통해서 사용자명과 비밀번호를 변경할 수 있으며 엔드포인트 접근에 대한 보안권한을 변경할 수 있다. 예를 들어, ```application.properties```를 다음과 같이 설정할 수 있다:

```
security.user.name=admin
security.user.password=secret
management.security.role=SUPERUSER
```

### 41.2. 관리 서버컨텍스트패스 변경
모든 관리용 엔드포인트 그룹을 단일 경로로 사용하는 것은 유용한 편이다. 예를 들어, 애플리케이션에서 이미 ```/info``` 를 다른 목적으로 사용하고 있다고 하자. ```management.contextPath``` 속성을 사용하여 관리 엔드포인트의 접두사를 설정할 수 있다.

```
management.context-path=/manage
```

```application.properties``` 에 사용했을 때 엔드포인트는 ```/{id}``` 에서 ```/manage/{id}```로 변경될 것이다(예: ```/manage/info```).

### 41.3. 관리 서버포트 변경<a name="41.3. 관리 서버포트 변경"></a>
기본 HTTP 포트를 사용하는 노출된 관리 엔드포인트들은 클라우드 배포시 고려사항이 있다. 그러나, 애플리케이션을 자신의 데이터센터 내에서 실행할 때에는 다른 HTTP 포트를 사용하여 엔드포인트 노출을 선호할 수 있다.

```management.port``` 속성을 사용하여 HTTP 포트를 변경할 수 있다.

```
management.port=8081
```

관리포트는 방화벽에 의해 보호되는 경우가 잦으며, 공개적으로 노출하지 않으면 관리 엔드포인트에 대한 보안을 필요로 하지 않을 것이다, 주 애플리케이션도 안전하다.스프링 시큐리티를 사용하는 경우, 관리 보안을 다음과 같이 비활성화할 수 있다.

```
management.security.enabled=false
```

스프링 시큐리티가 클래스패스 상에 없다면 위에서 처럼 관리보안을 명시적으로 비활성화할 필요는 없지만, 보안상 취약해질 수 있다.

### 41.4. 관리 서버주소 변경<a name="41.4. 관리 서버주소 변경"></a>
```management.address``` 속성을 설정하면 관리 엔드포인트의 주소를 변경할 수 있다.내부 혹은 ops-facing 혹은 ```localhost``` 만 접근하길 원하는 경우에 유용하다.

> 노트:
다른 주소로 접근하고자 할 경우에는 포트는 메인 서버 포트와 달라야 한다.

```application.properties``` 예제는 원격에서 관리 접근을 허용하지 않는다.

```
management.port=8081
management.address=127.0.0.1
```

### 41.5. HTTP 엔드포인트 비활성화<a name="41.5. HTTP 엔드포인트 비활성화"></a>
만약 HTTP를 통해서 엔드포인트가 노출되는 것을 원하지 않는다면 포트에 ```-1```을 설정하면 된다:
```
management.port=-1
```

### 41.6. 상태 엔드포인트에 대한 무기명 접근 제한<a name="41.6. 상태 엔드포인트에 대한 무기명 접근 제한"></a>
health 엔드포인트를 통해 노출되는 정보는 익명으로 접근했는가에 따라 달라진다. 익명으로 접근했을 경우 기본적으로 서버의 건강상태는 ```UP``` 혹은 ```DOWN``` 만 노출될 뿐 이외의 상세내용들은 감춰진다. 더욱이 익명으로 접근했을 경우의 응답은 서비스 거부 공격에 엔드포인트가 이용되는 것을 방지하기 위해 설정된 주기 동안의 캐시처리된 것이다. ```endpoints.health.time-to-live ``` 속성은 밀리세컨드 단위로 캐싱주기를 설정할 때 사용된다. 기본적으로 1000ms, 즉 1초로 설정된다.

앞에서 설명했던것처럼 익명사용자에 대한 health 엔드포인트에 대한 모든 권한을 허용하지 않도록 설정할 수 있다. ```endpoints.health.sensitive```를 ```false``` 로 설정하면 된다.

## 42. JMX를 통한 모니터링 및 관리<a name="JMX를 통한 모니터링 및 관리"></a>
자바 관리 확장(Java Management Extension, JMX)는 애플리케이션에 대한 모니터링과 관리에 대한 표준 메카니즘을 제공한다. 스프링부트는 기본적으로 ```org.springframework.boot``` 도메인 하위의 JMX MBeans에 관한 관리 엔드포인트를 제공한다.

### 42.1. MBean 이름 변경<a name="MBean 이름 변경"></a>
MBean의 이름은 항상 엔드포인트의 ```id```를 기반으로 생성된다. 예를 들어 ```health``` 엔드포인트는 ```org.springframework.boot/Endpoint/HealthEndpoint```를 기반으로 하고 있다.

애플리케이션에 스프링 ```ApplicationContext```을 한개이상 포함하고 있는 경우 이름이 충돌하는 것을 목격할 수 있을 것이다. 이 문제를 해결하는 방법은 ```endpoints.jmx.uniqueName``` 속성을 ```true``로 설정하여 이름을 항상 유일하게 하는 것이다.

또한 노출되는 엔드포인트 하위의 JMX 도메인을 변경할 수 있다. 여기 ```application.properties```에 설정하는 예제가 있다:

```
endpoints.jmx.domain=myapp
endpoints.jmx.uniqueNames=true
```

### 42.2. JMX 엔드포인트 비활성화<a name="JMX 엔드포인트 비활성화"></a>
만약 JMX 엔드포인트 노출을 원하지 않는 경우에는 ```spring.jmx.enabled``` 속성을 ```false```로 설정하면 된다:

```
spring.jmx.enabled=false
```

### 42.3. JMX용 Jolokia를 HTTP를 통해서 사용<a name="JMX용 Jolokia를 HTTP를 통해서 사용"></a>
Jolokia는 JMX beans 에 접근할 수 있는 대안방식을 가지고 있는 JMX-HTTP 브릿지다. Jolokia를 사용하려면, ```org.jolokia:jolokia-core``` 의존성을 포험시키면 된다. 예를 들어 메이븐을 사용하는 경우에는 다음과 같이 추가하면 된다:

```xml
<dependency>
    <groupId>org.jolokia</groupId>
    <artifactId>jolokia-core</artifactId>
 </dependency>
```

Jolokia는 사용중인 HTTP 서버에 ```/jolokia``` 로 접근할 수 있다.

#### 42.3.1. Jolokia 변경<a name="Jolokia 변경"></a>
Jolokia는 서블릿 파라메터를 이용해서 설정하는 다양한 방식을 가지고 있다. 스프링부트는 ```application.properties```를 통해서 설정할 수 있는데, ```jolokia.confg.``` 접두사를 통해 쉽게 할 수 있다:

```
jolokia.config.debug=true
```

#### 42.3.1. Jolokia 비활성화
스프링부트에서 Jolokia를 사용하지 않을 경우, ```endpoints.jolokia.enabled```를 ```false```로 설정하면 된다:

```
endpoints.jolokia.enabled
```

## 43. <a name="리모트쉘을 사용하여 모니터링 및 관리">리모트쉘을 사용하여 모니터링 및 관리</a>
스프링부트는 'CRaSH'라고 불리는 자바 쉘을 제공한다. CRaSH를 이용해서 애플리케이션 안에서 ```ssh``` 혹은 ```telnet``` 을 사용할 수 있다. 리모트쉘을 사용하려면 ```spring-boot-starter-remote-shell``` 의존성을 추가하면 된다:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-remote-shell</artifactId>
</dependency>
```

> 팁: 텔넷 접근을 활성화하려면 ```org.crsh:crsh.shell.telnet``` 의존성이 추가적으로 필요하다.

### 43.1. <a name="리모트쉘 연결">리모트쉘 연결</a>
리모트쉘의 기본 연결포트는 ```2000```번이다. 기본설정된 사용자명은 ```user``` 이고 기본 패스워드는 불규칙하게 생성되어 로그출력으로 노출된다. 만약 스프링시큐리티를 애플리케이션에 사용한다면, 쉘은 기본설정에 의해 (같은 설정)[#보안]을 사용할 것이다. 그렇지 않다면 다음과 같은 메시지와 함께 간단한 인증절차를 제공할 것이다:

```
Using default password for shell access: ec03e16c-4cf4-49ee-b745-7c8255c1dd7e
```

리눅스와 OSX 사용자는 ```ssh```를 사용하여 리모트쉘에 접근할 수 있으며, 윈도우 사용자는 [PuTTY](http://www.putty.org/)를 다운로드 받고 설치할 수 있다.

```
$ ssh -p 2000 user@localhost

user@localhost's password:
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::  (v1.2.0.BUILD-SNAPSHOT) on myhost
```

```help```를 입력하면 명령어 목록을 볼 수 있다. 스프링부트는 ```metrics```, ```beans```, ```autoconfig``` 그리고 ```endpoint``` 명령을 제공한다.

#### 43.1.1. <a name="리모트쉘 자격credentials">리모트쉘 자격credentials</a>
```shell.auth.simple.user.name``` 와 ```shell.auth.simple.user.password``` 속성을 사용하여 연결인증 정보를 변경할 수 있다. 또한 스프링시큐리티의 ```AuthenticationManager```를 사용하여 로그인 정책을 제어할 수 있다. 자세한 사항은  [CrshAutoConfiguration](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/actuate/autoconfigure/CrshAutoConfiguration.html) and [ShellProperties](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/actuate/autoconfigure/ShellProperties.html) Javadoc을 살펴보자.

### 43.2. <a name="리모트쉘 확장">리모트쉘 확장</a>
리모트쉘은 흥미로운 부분들을 확장가능하다.

#### 43.2.1. <a name="리모트쉘 명령어">리모트쉘 명령어</a>
리모트쉘은 그루비나 자바를 사용하여 쉘 명령어를 추가할 수 있다(보다 자세한 사항은 CRaSH 문서를 보자). 기본적으로 스프링부트는 다음의 위치에서 명령어들을 검색한다.
* ```classpath*:/commands/**```
* ```classpath*:/crash/commands/**```

> 팁: ```shell.commandPathPatterns``` 속성을 통해서 검색설정을 변경할 수 있다.

여기 ```src/main/resources/commands/hello.groovy``` 를 읽어오는 간단하게 'Hello world' 명령이 있다.

```groovy
package commands

import org.crsh.cli.Usage
import org.crsh.cli.Command

class hello {

    @Usage("Say Hello")
    @Command
    def main(InvocationContext context) {
        return "Hello"
    }

}
```

스프링부트는 명령으로 접근할 수 있는 ```InvocationContext``` 의 속성들을 추가할 수 있다.

| 속성명 | 설명 |
|--------|------|
|```spring.boot.version```|The version of Spring Boot|
|```spring.version``` | The version of the core Spring Framework|
|```spring.beanfactory``` | Access to the Spring BeanFactory |
|```spring.environment``` | Access to the Spring Environment |

#### 43.2.2. <a name="리모트쉘 플러그인">리모트쉘 플러그인</a>
새로운 명령을 추가하듯, CRaSH 쉘 기능들을 확장하는 것도 가능하다. ```org.crsh.plugin.CRaSHPlugin```을 확장한 모든 스프링뷘은 쉘에 자동으로 등록된다.

보다 자세한 정보는 [CRaSH reference documentation](http://www.crashub.org/) 을 통해서 확인하길 바란다.

## 44. <a name="측정">측정</a>
스프링부트 액추에이터는 'gauge'와 'counter' 측정 서비스를 제공한다. 'gauge'는 single value를 기록하고 'counter'는 delta(증가 혹은 감소)를 기록한다. 스프링부트 액추에이터는 또한 앞의 두 메카니즘이 기록하지 못하는 측정치를 확장구현할 수 있는 [PublicMetrics](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/endpoint/PublicMetrics.java) 인터페이스를 제공한다. 그 참고적인 예로 [SystemPublicMetrics](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/endpoint/SystemPublicMetrics.java)가 있다.

HTTP 요청은 자동으로 기록되어 측정되어, ```metrics``` 엔드포인트를 치면 다음과 유사한 내용을 확인할 수 있다:
```
{
    "counter.status.200.root": 20,
    "counter.status.200.metrics": 3,
    "counter.status.200.star-star": 5,
    "counter.status.401.root": 4,
    "gauge.response.star-star": 6,
    "gauge.response.root": 2,
    "gauge.response.metrics": 3,
    "classes": 5808,
    "classes.loaded": 5808,
    "classes.unloaded": 0,
    "heap": 3728384,
    "heap.committed": 986624,
    "heap.init": 262144,
    "heap.used": 52765,
    "mem": 986624,
    "mem.free": 933858,
    "processors": 8,
    "threads": 15,
    "threads.daemon": 11,
    "threads.peak": 15,
    "uptime": 494836,
    "instance.uptime": 489782,
    "datasource.primary.active": 5,
    "datasource.primary.usage": 0.25
}
```

HTTP 측정을 통해서 ```memory```, ```heap```, ```class loading```, ```processor``` and ```thread pool```에 관한 기본적인 정보를 볼 수 있다. 이 인스턴스의 루트(```/```) 그리고 ```/metrics``` 는 ```HTTTP 200``` 3번에서 20번 응답한다. 또한 ```root``` URL 에 대해서는 ```HTTP 401(인증되지 않음)```은 4번 반환한다. 더블 아스트릭스(star-start)는 스프링MVC 의 ```/**```(일반적인 정적 리소스)에 대응한다.

```guage```는 요청에 대한 최근 응답을 보여준다. 그래서 ```root```는 가장최근 ```2ms```의 것을, ```/metrics```는 가장최근 ```3ms```의 것을 응답한다.

> 설명: 이 예는 실제로 ```/metrics``` URL에 대해서 HTTP 를 통해 엔드포인트에 접근했을 때, ```metrics``` 응답을 설명한 것이다.

### 44.1. <a name="데이터소스 측정">데이터소스 측정</a>
다음의 측정은 애플리케이션에 정의되어있는 ```DataSource``` 설정을 탐색한다.
* 최대 커넥션 수(```datasource.xxx.max```)
* 최소 커넥션 수(```datasource.xxx.min```)
* 활동 커넥션 수(```datasource.xxx.active```)
* 커넥션 풀에서 현재 사용중인 상태(```datasource.xxx.usage```)

```datasource``` 을 접두어로 선언된 모든 데이터 소스 측정을 제공한다. 접두어는 각각의 데이터소스을 구분지을 수 있다:
* 만약 데이터소스가 primary 데이터 소스(한개만 사용하거나 여러 개 중에 ```@Primary``` 애노테이션으로 표기한)가 있다면, 접두어는 ```datasource.primary```가 될 것이다.
* ```dataSource```로 끝나는 빈이름을 가진 경우, 접두어는 빈의 이름에서 ```datasource```를 제거한 이름을 가진다(예: ```batchDataSource```의 경우 ```datasource.batch```)가 될 것이다.
* 그 외의 경우에는, 빈의 이름을 사용한다.

```DataSourcePublicMetrics``` 사용자 정의 버전으로 빈을 등록하여 일부 또는 모든 기본값을 대체할 수 있다. 기본적으로 스프링부트는 지원가능한 모든 데이터소스에 대한 메타데이터를 제공한다. 지원대상 외의 좋아하는 데이터소스를 지원하는 ```DataSourcePoolMetadataProvider``` 빈을 추가할 수도 있다. 예로 ```DataSourcePoolMetadataProvidersConfiguration```를 살펴보라.

### 44.2. <a name="측정 기록">측정 기록</a>
[CounterService](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/metrics/CounterService.java)와 [GaugeService](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/metrics/GaugeService.java)의 측정기록을 빈에서 사용하기 위해 주입할 수 있다. ```CounterService``` 는 ```increment```, ```decrement``` 와 ```reset``` 메서드를 확장할 수 있다; ```GaugeService 는 ```submit``` 메서드를 제공한다.

여기 메서드가 호출된 횟수를 카운트하는 간단한 예제가 있다
```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.actuate.metrics.CounterService;
import org.springframework.stereotype.Service;

@Service
public class MyService {

    private final CounterService counterService;

    @Autowired
    public MyService(CounterService counterService) {
        this.counterService = counterService;
    }

    public void exampleMethod() {
        this.counterService.increment("services.system.myservice.invoked");
    }

}
```

> 팁: 측정명은 어떤 문자열로도 사용가능하지만 저장/그래프 기술을 선택할 때 가이드라인에 따르기 바란다. Graphite를 위한 가이드라인이 좋은 편인데 [Matt Aimonetti's Blog](http://matt.aimonetti.net/posts/2013/06/26/practical-guide-to-graphite-monitoring/)에서 살펴볼 수 있다.

### 44.3. <a name="공개 측정 추가">공개 측정 추가</a>
```PublicMetrics``` 구현체 빈을 추가 등록해놓으면, 측정 엔드포인트가 호출될때마다 계산되는 추가 측정요소를 추가할 수 있다. 기본적으로, 모든 빈들은 엔드포인트에 의해 수집된다. ```MetricsEndpoint```을 정의하여 쉽게 변경할 수 있다.

### 44.4. <a name="측정 레파지토리"></a>측정 레파지토리
측정 서비스 구현체는 항상 [MetricRepository](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/metrics/repository/MetricRepository.java)와 연결된다. ```MetricRepository```는 측정정보를 저장하고 반환한다. 스프링 부트는 ```InMemoryMetricRepository``` 와 ```RedisMetricRepository```를 제공한다(기본은 in-memory repository다) 그러나 우리가 작성한 것도 사용가능하다. ```MetricRepository``` 인터페이스는 ```MetricReader``` 와 ```MetricWriter``` 인터페이스 보다 높은 위치에 있다. 보다 자세한 내용은 [Javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/actuate/metrics/repository/MetricRepository.html)을 살펴보자.

```MetricRepository```를 통해 앱의 백엔드로 바로 저장하는 것을 아무도 제지하지 않지만, 기본으로 ```InMemoryMetricRepository```(힙heap 사용이 꺼려진다면 ```Map``` 인스턴스를 수정할 수 있다) 사용을 권장하고 규칙으로 잡을 내보내는 백엔드 저장소를 선호한다. 다른 방법으로는 측정치를 메모리에 버퍼링을 통해 얻고 배치나 네트워크 통신량이 감소하는 때에 내보내는 것이다. 스프링 부트는 ```Exporter``` 인터페이스를 제공하고 그것에서 시작하는 기본적인 구현체들을 제공한다.

### 44.5. <a name="Coda Hale 측정"></a>Coda Hale 측정
[Coda Hale 'Metrics' 라이브러리](http://metrics.codahale.com/)의 사용자는 스프링부트 측정이 ```com.codahale.metrics.MetricRegistry```으로 출판한 것들을 자동으로 찾아낼 것이다. 기본 ```com.codahale.metrics.MetricRegistry``` 스프링빈은 ```com.codahale.metrics:metrics-core``` 의존성을 정의하면 생성된다. 변경이 필요하다면 ```@Bean``` 인스턴스를 추가등록할 수 있다.

사용자는 적절한 형태로 자신의 측정에 대한 이름을 덥두어로 Coda Hale metrics 을 만들 수 있다(예: ```histogram.*```, ```meter.*```).

### 44.6. <a name="메시지 채널 통합"></a>메시지 채널 통합
만약에 '스프링 메시징' jar 파일이 클래스패스 상에 있다면 ```metricsChannel```이라 불리는 ```MessageChannel```이 자동으로 생성된다(이미 존재하지 않는다면). 모든 측정 업데이트 이벤트는 채널을 통해 'messages'를 출판Publishing하여 추가한다. 클라이언트에서는 이 채널을 구독Subscribe하여 분석이나 액션을 추가할 수 있다.

## 45. <a name="감시auditing"></a>감시auditing
스프링부트 액추에이터는 스프링 시큐리티의 동작('인증 성공', '실패' 그리고 기본적인 '접근 거부')에서 발생하는 이벤트 들을 유연하게 감시할 수 있다. 이것은 리포팅에 매우 유용하며 인증 실패를 기반으로 한 잠금해제 정책을 구현할 수 있다.

또한 비즈니스 이벤트를 위한 감시 서비스 사용을 고려할 수 있다. 컴포넌트 안에 ```AuditEventRepository```를 주입하거나 스프링의 ```ApplicationEventPublisher```을 통해서 ```AuditApplicationEvent``` 를 간단하게 발급할 수 있다(```ApplicationEventPublisherAware``` 사용).

## 46. 추적Tracing<a name="추적Tracing"></a>
추적은 모든 HTTP 요청에 대해서 자동적으로 활성화된다. ```trace``` 엔드포인트로 볼 수 있으며 최근 요청들에 대해 기본적인 정보를 제공한다.
```json
[{
    "timestamp": 1394343677415,
    "info": {
        "method": "GET",
        "path": "/trace",
        "headers": {
            "request": {
                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
                "Connection": "keep-alive",
                "Accept-Encoding": "gzip, deflate",
                "User-Agent": "Mozilla/5.0 Gecko/Firefox",
                "Accept-Language": "en-US,en;q=0.5",
                "Cookie": "_ga=GA1.1.827067509.1390890128; ..."
                "Authorization": "Basic ...",
                "Host": "localhost:8080"
            },
            "response": {
                "Strict-Transport-Security": "max-age=31536000 ; includeSubDomains",
                "X-Application-Context": "application:8080",
                "Content-Type": "application/json;charset=UTF-8",
                "status": "200"
            }
        }
    }
},{
    "timestamp": 1394343684465,
    ...
}]
```

### 46.1. 추적 변경<a name="추적 변경"></a>
추가적으로 이벤트들에 대한 추적이 필요하다면 스프링 빈 안에 [TraceRepository](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/trace/TraceRepository.java) 를 주입하면 된다. ```add``` 메서드에 싱글 ```Map``` 구조를 전달하면 JSON으로 컨버팅되고 로그도 남는다.

기본적으로 ```InMemoryTraceRepository```을 사용하면 최근 100개 이벤트를 저장한다. 이 부분을 확장하고자 한다면 ```InMemoryTraceRepository``` 인스턴스를 정의할 수 있다. 또한 필요하다면 ```TraceRepository```을 구현하는 방법도 선택할 수 있다.

## 47. 프로세스 모니터링<a name="프로세스 모니터링"></a>
스프링 액추에이터는 프로세스 모니터링에 파일들을 생성하는 유용한 클래스들을 찾아볼 수 있다:
* ```ApplicationPidFileWriter``` 애플리케이션의 PID 파일을 생성한다(기본적으로  ```application.pid``` 파일을 애플리케이션 디렉토리에 생성한다).
* ```EmbeddedServerPortFileWriter``` 내장 서버의 포함한 파일을 생성한다(기본적으로 ```application.port``` 파일을 애플리케이션 디렉토리에 생성).

이 writer들은 기본적으로 활성화되지 않지만 아래에 설명된 방법들 중 하나로 활성화할 수 있다.

### 47.1. 설정 확장<a name="설정 확장"></a>
```META-INF/spring.factories``` 파일을 두면 리스너들을 활성화한다:
```
org.springframework.context.ApplicationListener=\
org.springframework.boot.actuate.system.ApplicationPidFileWriter,
org.springframework.boot.actuate.system.EmbeddedServerPortFileWriter
```

### 47.2. 작성<a name="작성"></a>
```SpringApplication.addListeners(…​)``` 메서드로 호출하여 리스너를 활성화하고 ```Writer``` object를 전달하면 된다. 이 방법은 ```Writer``` 생성자를 이용해서 파일명과 경로를 변경하는 것이 가능하다.

## 48. 다음 읽을거리
만약 이번 장에서 다뤄진 개념들을 좀 더 살펴보고자 한다면 액츄에이터 [예제 애플리케이션](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples)들을 살펴보라. 거기에 더해서 [Graphite](http://graphite.wikidot.com/) 같은 그래프 도구에 대해서도 읽어보십시오.

혹은, 계속 읽는다면, '[클라우드 배포](#클라우드 배포)' 혹은 스프링부트의 [빌드툴 플러그인](#빌드툴 플러그인)를 심도있게 다루는 부분으로 넘어갈 수도 있다.

# VI. 클라우드 배포<a name="클라우드 배포"></a>
## 49. Cloud Foundry<a name="Cloud Foundry"></a>
### 49.1. 서비스 연결
## 50. Heroku<a name="Heroku"></a>
## 51. CloudBees<a name="CloudBees"></a>
## 52. Openshift
## 53. Google App Engine
## 54. 다음 읽을거리

# VII. 스프링부트 CLI<a name="스프링부트 CLI"></a>
스프링을 써서 빨리 개발하고 싶을 때 스프링부트 CLI를 쓸 수 있다. 스프링부트 CLI는 상투적으로 반복하는 코드를 잔뜩 쓰지 않고도, 익숙한 자바같은 문법을 쓰는 그루비 스크립트를 실행할 수 있게 해준다. 사용자만의 고유한 명령을 만들거나 새 프로젝트를 위한 환경을 빠르게 갖추려고 할 때에(bootstrap a new project) 쓸 수 있다.

## 54. CLI 설치
스프링부트 CLI는 수동으로 설치할 수 있다. GVM(그루비 환경관리자)이나 OSX 사용자라면 Homebrew를 써서 설치한다. 더 포괄적인 설치 지침은 [섹션 10.2, "스프링부트 CLI 설치하기"](#CLI를 이용한 설치)에서 보도록 하자.

## 55. CLI 사용
CLI를 설치하고 나면 `spring`이라고 쳐서 실행할 수 있다. 아무런 인자도 주지않고 `spring`을 실행하면 다음과 같이 간단한 도움말 화면을 보게 될 것이다 :
```
$ spring
usage: spring [--help] [--version]
       <command> [<args>]

Available commands are:

  run [options] <files> [--] [args]
    Run a spring groovy script

  ... more command help is shown here
```
`help`로 지원하는 명령을 자세하게 살펴볼 수 있다. 예를 들면 :
```
$ spring help run
spring run - Run a spring groovy script

usage: spring run [options] <files> [--] [args]

Option                     Description
------                     -----------
--autoconfigure [Boolean]  Add autoconfigure compiler
                             transformations (default: true)
--classpath, -cp           Additional classpath entries
-e, --edit                 Open the file with the default system
                             editor
--no-guess-dependencies    Do not attempt to guess dependencies
--no-guess-imports         Do not attempt to guess imports
-q, --quiet                Quiet logging
-v, --verbose              Verbose logging of dependency
                             resolution
--watch                    Watch the specified file for changes
```
`version` 명령으로 사용하고 있는 스프링부트 버전이 어떤 것인지 빠르게 체크할 수 있다.
```
$ spring version
Spring CLI v1.2.0.RELEASE
```

### 55.1. CLI를 이용해서 애플리케이션 실행
`run` 명령으로 그루비 소스코드를 컴파일하고 실행할 수 있다. 스프링부트 CLLI는 그루비를 포함하고 있으므로 별다른 그루비를 설치할 필요가 없다.
아래 그루비로 된 "hello world" 웹 어플리케이션 예를 보자 :

*hello.groovy*.
```groovy
@RestController
class WebApplication {

    @RequestMapping("/")
    String home() {
        "Hello World!"
    }

}
```
어플리케이션을 컴파일하고 실행하려면 다음과 같이 입력한다 :
```
$ spring run hello.groovy
```
어플리케이션 명령행 인자를 주려면 `--`를 "spring" 명령과 분리하는 데 사용하도록 한다. 즉, 다음과 같다.
```
$ spring run hello.groovy -- --server.port=9000
```
JVM 명령행 인자를 설정하는 데에는 `JAVA_OPTS` 환경변수를 사용할 수 있다. 즉,
```
$ JAVA_OPTS=-Xmx1024m spring run hello.groovy
```
#### 55.1.1. "grab" 의존성 추정
표준 그루비는 서드 파티 라이브러리에 대한 의존성을 선언할 수 있게 해주는 `@Grab` 어노테이션을 포함하고 있다.
빌드 도구를 사용하지 않고서 메이븐이나 그래들과 같은 방법으로 그루비가 jar 파일을 다운로드 하게 해주는 유용한 방법이다.

스프링 부트는 이 방법을 좀 더 확장하여, 코드를 토대로 `grab`할(+가져올) 라이브러리를 추론하려고 시도할 것이다. 예를 들어, `@RestController`어노테이션을 사용하고 있는 `WebApplication` 코드로 "`Tomcat`"과 "`Spring MVC`를 가져오게 될 것이다.

다음은 "`grab hints`"(+가져오기 힌트)로 쓰이는 항목이다 :

| 항목 | 가져오는 것|
|--- | ---|
|`JdbcTemplate`, `NamedParameterJdbcTemplate`, `DataSource` |JDBC 어플리케이션|
|`@EnableJms` |JMS 어플리케이션|
|`@EnableCaching` | Caching abstraction.|
|`@Test` |JUnit.|
|`@EnableRabbit` |RabbitMQ.|
|`@EnableReactor` |Project Reactor.|
|확장`Specification` |Spock test.|
|`@EnableBatchProcessing` |Spring Batch.|
|`@MessageEndpoint` `@EnableIntegrationPatterns` |Spring Integration.|
|`@EnableDeviceResolver` |Spring Mobile.|
|`@Controller` `@RestController` `@EnableWebMvc` |Spring MVC + Embedded Tomcat.|
|`@EnableWebSecurity` |Spring Security.|
|`@EnableTransactionManagement` |Spring Transaction Management.|

 > 스프링부트 CLI 소스코드에서 사용자화[customization]가 어떻게 적용되는지 이해하려면 [`CompilerAutoConfiguration`](https://github.com/spring-projects/spring-boot/blob/v1.2.0.RELEASE/spring-boot-cli/src/main/java/org/springframework/boot/cli/compiler/CompilerAutoConfiguration.java)의 서브클래스를 보라.

#### 55.1.2. 추정한 "grab"의 coordinates(+groupId:artifactId:packaging:version)
스프링 부트는 그루비의 표준 `@Grab` 지원을 확장하여 그룹이나 버전정보 없이 의존성을 표기할 수 있도록 허용한다. (+스프링 부트의 `@Grab`은) artifact의 그룹과 버전 정보를 추정하기 위해 스프링 부트의 기본 의존성 메타데이터를 찾아볼 것이다.좌표기본 메타데이터는 현재 사용하고 있는 CLI 버전에 묶여있다는 것을 명심하자 - 이것은 새 버전 CLI로 이동했을 때에만 바뀌므로 사용자가 의존성의 버전이 바뀌는 것을 제어하도록 해준다.
기본 메타데이터에 포함된 의존성과 버전에 대한 표는 [부록](#dependency-verions)에서 찾을 수 있다.

#### 55.1.3. 기본 import문
그루비 코드 크기를 줄이기 위해 몇몇 `import`문은 자동으로 포함된다.
위에서 봤던 예에서 어떻게 `import`문이나 클래스를 표시한 이름을 쓰지 않고 `@Component`, `@RestController`와 `@RequestMapping`을 불러 썼는지 주의해서 살펴보라.

 > 많은 스프링 어노테이션이 `import`문 없이 동작할 것이다. import를 추가하기 전에, 어플리케이션을 실행해서 어떤 것이 실패하는 지 살펴보라.

#### 55.1.4. 자동 main 메소드
비슷한 자바 어플리케이션과 다르게, `Groovy`스크립트에는 `public static void main(String[] args)`를 넣어둘 필요가 없다. `SpringApplication`은 자동으로 만들어져서 컴파일한 사용자 코드와 함께 `source`로 동작할 것이다.

#### 55.1.5. 사용자[Custom] "`grab`" 메타데이터
스프링부트는 스프링부트의 기본 메타데이터를 무시하고[overrides] 사용자가 지정한 의존성 메타데이터를 사용할 수 있도록 `@GrabMetadata` 어노테이션을 새롭게 제공한다.
이 메타데이터는 어노테이션을 사용해서 지정할 수 있으며 하나 혹은 그 이상 프로퍼티 파일[properties files]을 어노테이션에 제공해줄 수 있다.((+프로퍼티 파일은)메이븐 저장소에 있는 `properties` `type` 식별자가 붙은 파일)

각 프로퍼티 파일에 개별 항목은 `group:module=version`형식이어야 한다.

예를 들면 다음 선언에서는:
```java
@GrabMetadata("com.example.custom-versions:1.0.0")
```
메이븐 저장소 `com/example/custom-versions/1.0.0/` 아래에서 `custom-versions-1.0.0.properties`를 가져올 것이다.

어노테이션에 명시된 다중 프로퍼티 파일은 선언된 순서대로 적용될 것이다. 예로 :
```
@GrabMetadata(["com.example.custom-versions:1.0.0",
    "com.example.more-versions:1.0.0"])
```
은 `more-versions`의 프로퍼티가 `custom-versions`의 프로퍼티를 [override]하게 될 것이다.

`@Grab`을 쓸 수 있는 곳이면 어디나 `@GrabMetadata`를 쓸 수 있다. 하지만 메타데이터 순서에 일관성을 지키기 위해서 `@GrabMetadata`는 어플리케이션에서 최대 한 번만 사용하는 게 낫다.
(스프링 부트의 상위집합인)유용한 의존성 메타데이터의 원천은 [Spring IO Platform](http://platform.spring.io/)이다. 예를 들면 다음과 같다 :
```java
@GrabMetadata('io.spring.platform:platform-versions:1.0.4.RELEASE')
```
### 55.2 코드 테스트하기
`test` 명령은 어플리케이션을 컴파일하고 테스트를 실행할 수 있도록 해준다. 보통 다음과 같이 사용한다.

```
	$ spring test app.groovy tests.groovy
	Total: 1, Success: 1, : Failures: 0
	Passed? true
```

이 예제에서는 `tests.groovy`가 JUnit `@Test` 메소드나 Spock `Specipication` 클래스를 포함하고 있다. 모든 공통 프레임워크 어노테이션과 스태틱 메소드는 `import`하지 않아도 사용할 수 있을 것이다.
위에서 사용한 이 `tests.groovy` 파일은 JUnit으로 작성했다 :

```java
	class ApplicationTests {

		@Test
		void homeSaysHello() {
			assertEquals("Hello World!", new WebApplication().home())
		}

	}
```
 > 테스트용 소스 파일이 여러 개 있다면 `test`디렉토리 안에 넣어두는 편을 선호할 것이다.

### 55.3. 소스 파일이 여러 개인 어플리케이션의 경우
파일 입력을 받아들이는 모든 명령어는 "`shell globbing`"(+정규식으로 파일을 찾아서 실행함)을 사용할 수 있다. 같은 디렉토리에서 파일 여러 개를 쉽게 실행하도록 해준다. 다음과 같다 :

```
	$ spring run *.groovy
```

"`test`"나 "`spec`"코드를 메인 어플리케이션 코드와 분리하고 싶다면 이 방법도 쓸모있을 것이다:

```
	$ spring test app/*.groovy test/*.groovy
```

### 55.4. 애플리케이션 패키징 하기
어플리케이션을 독립 실행가능한 jar 파일로 패키징하려면 `jar` 명령을 사용하면 된다. 다음과 같다 :

```
	$ spring jar my-app.jar *.groovy
```

이렇게 만들어진 jar는 어플리케이션을 컴파일하면서 얻은 클래스와 어플리케이션에 필요한 모든 의존성을 포함하고 있으므로, `java -jar`명령을 사용하여 실행할 수 있다. 이 jar 파일은 어플리케이션 클래스패스의 (+라이브러리 참조)항목들도 포함하고 있다. `--include`와 `--exclude`를 써서 jar 에 추가할 경로를 명시할 수 있다. (두 옵션 모두 경로를 쉼표(,)로 구분하고, 이 옵션이 기본적으로 설정하는 경로에서 빼고 싶은 경로는 "`+`"(+exclude의 경우),"`-`"(+include의 경우)를 해당 경로 앞에 쓴다. 기본적으로 포함하는 경로는 다음과 같다 :

```
	public/**, resources/**, static/**, templates/**, META-INF/**, *
```
그리고 아래 경로는 기본적으로 제외한다.

```
	.*, repository/**, build/**, target/**, **/*.jar, **/*.groovy
```

더 자세한 정보는 `spring help jar`의 결과를 보라.

### 55.5. 새로운 프로젝트 초기화 하기
`init` 명령은 쉘을 나가지 않고도 [start.spring.io](https://start.spring.io)를 이용해서 새 프로젝트를 만들 수 있게 해준다. 예 :

```
	$ spring init --dependencies=web,data-jpa my-project
	Using service at https://start.spring.io
	Project extracted to '/Users/developer/example/my-project'
```

이렇게 하면 `my-project`디렉토리를 만들고 여기에 `spring-boot-starter-web` 과`spring-boot-starter-data-jpa`를 이용하여 메이븐 기반 프로젝트를 만든다. `--list`플래그를 이용해서 제공하는 여러 기능 목록을 볼 수 있다.(+Project types, Parameters, Supported dependencies 목록이 나온다.)

```
	$ spring init --list
	=======================================
	Capabilities of https://start.spring.io
	=======================================

	Available dependencies:
	-----------------------
	actuator - Actuator: Production ready features to help you monitor and manage your application
	...
	web - Web: Support for full-stack web development, including Tomcat and spring-webmvc
	websocket - Websocket: Support for WebSocket development
	ws - WS: Support for Spring Web Services

	Available project types:
	------------------------
	gradle-build -  Gradle Config [format:build, build:gradle]
	gradle-project -  Gradle Project [format:project, build:gradle]
	maven-build -  Maven POM [format:build, build:maven]
	maven-project -  Maven Project [format:project, build:maven] (default)

	...
```

`init` 명령은 여러가지 옵션을 지원하는데, `help`를 이용해서 더 자세한 정보를 볼 수 있다(+`prompt > spring --help init`). 예를 들면 다음 명령은 java 8을 이용하고 `war`로 패키징하는 그래들 프로젝트를 생성한다.

----
	$ spring init --build=gradle --java-version=1.8 --dependencies=websocket --packaging=war sample-app.zip
	Using service at https://start.spring.io
	Content saved to 'sample-app.zip'
----

### 55.6. 내장형 쉘 사용하기
스프링부트는 BASH와 zsh 쉘을 위한 명령 완성 스크립트를 포함하고 있다. BASH나 zsh 쉘을 사용하지 않는다면(아마도 윈도우 사용자) `shell` 명령으로 통합된 쉘을 띄울 수 있다.

```
	$ spring shell
	*Spring Boot* (v{spring-boot-version})
	Hit TAB to complete. Type \'help' and hit RETURN for help, and \'exit' to quit.
```

내장형 쉘 안에서 다른 명령도 직접 실행시킬 수 있다 :

```
	$ version
	Spring CLI v{spring-boot-version}
```

내장형 쉘은 `tab` 완성과 함께 ANSI 색으로 출력하는 것도 지원한다. 내장형 쉘이 아닌, 쉘 본래 명령을 실행하려면 앞에 `$`를 붙이면 된다.(+현재 Spring CLI v1.2.6.RELEASE 에서는 `!`이다.) `ctrl-c`를 누르면 내장형 쉘을 종료한다.

### 55.7 CLI에 확장 추가하기
`install` 명령으로 CLI에 확장을 추가할 수 있다. `group:artifact:version` 형태로 된 artifact coordinates를 한 개 이상 지정할 수 있다. 예 :

```
	$ spring install com.example:spring-boot-cli-extension:1.0.0.RELEASE
```

사용자가 지정한 artifacts를 인스톨하면서 해당 artifacts의 모든 의존성 또한 같이 설치될 것이다.

의존성을 제거하려면 `uninstall` 명령을 사용한다. `install`처럼 artifact coordinates를 한 개 이상 지정할 수 있다. 예 :

```
	$ spring uninstall com.example:spring-boot-cli-extension:1.0.0.RELEASE
```

이렇게 하면 사용자가 지정한 artifact와 이 artifact의 의존성도 함께 제거될 것이다.

모든 의존성을 제거하려면 `--all` 옵션을 사용한다 :

```
	$ spring uninstall --all
```

## 56. 그루비 빈즈 DSL을 통해서 애플리케이션 개발
스프링 프레임워크 4.0 은 "DSL" ```beans{}``` 를 지원하도록 해준다. 

```
@Configuration
class Application implements CommandLineRunner {

    @Autowired
    SharedService service

    @Override
    void run(String... args) {
        println service.message
    }

}

import my.company.SharedService

beans {
    service(SharedService) {
        message = "Hello World"
    }
}
```


## 57. 다음 읽을거리

# VIII. 빌드툴 플러그인<a name="빌드툴 플러그인"></a>
스프링부트는 메이븐과 그레들 플러그인을 위한 빌드툴 플러그인을 제공한다. 플러그인은 실행가능한 jar 압축을 포함한 다양한 기능을 제공한다. 이 섹션은 플러그인에 대한 보다 상세한 내용을 제공하고, 지원하지 않는 빌드 시스템에 대한 확장에도 도움이 될 것이다. 만약 바로 시작하려한다면, [III. 스프링부트 사용](#III. 스프링부트 사용)에서 [13. 빌드시스템](#13. 빌드 시스템) 을 읽어보기를 바란다.

## 59. 스프링부트 메이븐 플러그인<a name="스프링부트 메이븐 플러그인"></a>
[스프링부트 메이븐 플러그인](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/maven-plugin/)은, 실행가능한 jar 혹은 war 압축파일 압축기능과 부트앱 실행 기능을 제공한다. 메이븐3 부터 사용가능하다.
> 노트:
플러그인에 대한 보다 자세한 사항은 [스프링부트 메이븐 플러그인 사이트](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/maven-plugin/)를 참조하라.

### 59.1. 플러그인 추가<a name="59.1. 플러그인 추가"></a>
스프링부트 메이븐 플러그인은 ```pom.xml``` 에서 ```plugins``` 섹션에 다음의 내용을 간단히 추가하면 사용할 수 있다.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    <!-- ... -->
    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
                <version>1.2.0.BUILD-SNAPSHOT</version>
                <executions>
                    <execution>
                        <goals>
                            <goal>repackage</goal>
                        </goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>
</project>
```

이 설정은 메이븐의 생존주기 ```package``` 페이즈 동안 jar 혹은 war를 재압축한다. 다음의 ```target``` 디렉토리를 보면 original jar와 재압축된 jar 파일을 볼 수 있다:

```
$ mvn package
$ ls target/*.jar
target/myproject-1.0.0.jar target/myproject-1.0.0.jar.original
```

위 설정에서 ```<execution/>```을 포함시키지 않았어도 플러그인을 실행할 수 있다(하지만 ```package``` 골을 사용해야 한다). 예를 들어:

```
$ mvn package spring-boot:repackage
$ ls target/*.jar
target/myproject-1.0.0.jar target/myproject-1.0.0.jar.original
```

만약 마일스톤 혹은 스냅샷 버전을 사용한다면 ```pluginRepository``` 요소를 적절히 추가해야할 것이다:

```xml
<pluginRepositories>
    <pluginRepository>
        <id>spring-snapshots</id>
        <url>http://repo.spring.io/snapshot</url>
    </pluginRepository>
    <pluginRepository>
        <id>spring-milestones</id>
        <url>http://repo.spring.io/milestone</url>
    </pluginRepository>
</pluginRepositories>
```
### 59.2. 실행가능한 jar 와 war 파일 패키징<a name="59.2. 실행가능한 jar 와 war 파일 패키징"></a>
```pom.xml```에 추가된 ```spring-boot-maven-plugin```은 ```spring-boot:repackage``` 골이 사용될 경우 자동으로 압축파일을 재압축하여 실행가능하게 만든다. ```packaging``` 요소를 사용하여 jar 혹은 war 파일 빌드타입을 설정할 수 있다.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <!-- ... -->
    <packaging>jar</packaging>
    <!-- ... -->
</project>
```

```package``` 페이즈 동안에 스프링부트에 의해 존재하는 압축파일이 처리된다. 실행하고자 하는 메인클래스를 설정항목을 통해 정의하거나 ```Main-Class``` 속성을 메니페스트에 추가하는 방법을 통해 실행한다. 만약 메인 클래스를 정의하지 않았다면 플러그인은 클래스에서 ```public static void main(String[] args)``` 메서드를 탐색할 것이다.

빌드된 프로젝트 산출물을 실행하려면 다음과 같이 입력하면 된다:

```
$ mvn package
$ java -jar target/mymodule-0.0.1-SNAPSHOT.jar
```

war 파일을 빌드했을 경우에는 실행하거나 외부 컨테이너에 배포하는 경우에는 내장된 컨테이너의 의존성을 ```provided``` 로 정의해줘야 한다. 예:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <!-- ... -->
    <packaging>war</packaging>
    <!-- ... -->
    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
            <scope>provided</scope>
        </dependency>
        <!-- ... -->
    </dependencies>
</project>
```

> 팁:
배포가능한 war 파일을 어떻게 생성하는지 상세히 알고 싶다면 [75.1. 배포가능한 war 파일 생성](#75.1. 배포가능한 war 파일 생성) 섹션을 살펴보자.

보다 상세한 설정항목과 예는 [플러그인 안내 페이지](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/maven-plugin/)에서 볼 수 있다.

## 60. 스프링부트 그레들 플러그인<a name="60. 스프링부트 그레들 플러그인"></a>
스프링부트 그레들 플러그인은 그레들에서 스프링부트를 지원하도록 제공하며, 실행가능한 jar 혹은 war 파일을 압축하는 것을 허용하며, 스프링부트 애플리케이션을 실행시키고 ```build.gradle```` 파일에서 사전 정의된 의존성을 제공하여 버전을 삭제할 수 있다.

### 60.1. 플러그인 추가<a name="60.1. 플러그인 추가"></a>
스프링부트 그레들 플러그인을 사용하려면 ```buildscript``` 의존성과 ```spring-boot``` 플러그인을 간단히 추가하면 된다:
```
buildscript {
    dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:1.2.0.BUILD-SNAPSHOT")
    }
}
apply plugin: 'spring-boot'

If you are using a milestone or snapshot release you will also need to add appropriate repositories reference:

buildscript {
    repositories {
        maven.url "http://repo.spring.io/snapshot"
        maven.url "http://repo.spring.io/milestone"
    }
    // ...
}
```

### 60.2. 버전 없이 의존성 정의<a name="60.2. 버전 없이 의존성 정의"></a>
```spring-boot``` 플러그인은 수정된 그레들 ```ResolutionStrategy```을 등록하여 "축복받은" 아티팩트의 의존성을 정의할 때 버전숫자를 생략하는 것을 허용한다. 이 기능의 사용법은, 정의된 의존성을 쉽게 사용할 수 있는, 버전숫자를 비우면 된다:

```
dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    compile("org.thymeleaf:thymeleaf-spring4")
    compile("nz.net.ultraq.thymeleaf:thymeleaf-layout-dialect")
}
```

> 노트:
선언된 ```spring-boot``` 그레들플러그인이 "축복받은" 의존성의 실체 버전을 결정한다(비드는 항상 반복적이기에 이를 보장한다). 항상 사용하고자 하는 실제 스프링부트 버전으로 스프링부트 플러그인의 버전을 설정해야 한다(역자주: 60.1. 에서 정의한 buildscript 에서 의존성 정의시 버전을 말함). 제공되는 버전의 자세한 항목들은 [부록](#E. 의존성 버전)을 살펴보기 바란다.

```spring-boot``` 플러그인은 정의되지 않은경우에만 정의된 버전을 제공한다. 아티팩트 정의에 플러그인에서 제공하는 것과 다른 버전을 사용하면, 항상 정의한 버전의 의존성으로 사용한다. 예를 들어:
```
dependencies {
    compile("org.thymeleaf:thymeleaf-spring4:2.1.1.RELEASE")
}
```

#### 60.2.1. 버전 관리 변경<a name="60.2.1. 버전 관리 변경"></a>
스프링부트의 "축복받은" 의존성으로부터 벗어나야할 경우 ```ResolutionStrategy```에서 사용하는 버전을 사용자 정의할 수 있다. ```versionManagement``` 설정을 사용하여 대안버전 메타데이터를 정의할 수 있다. 예를 들어:
```
dependencies {
    versionManagement("com.mycorp:mycorp-versions:1.0.0.RELEASE@properties")
    compile("org.springframework.data:spring-data-hadoop")
}
```

버전정보는 배포 레파지티로리 등록한 ```.properties``` 파일을 필요로 한다. 위에 예에서 ```mycorp-versions.properties``` 파일은 다음과 같다:
```
org.springframework.data\:spring-data-hadoop=2.0.0.RELEASE
```

프로퍼티즈 파일은 스프링부트의 기본값보다 우선하고, 필요한 경우 버전번호를 대체할 수 있다.

### 60.3. 기본적인 배제 원칙<a name="60.3. 기본적인 배제 원칙"></a>
그레들은 starter POMs를 사용할 때  예기치 않은 결과가 발생할 수 있기에 메이븐과는 다른 방법으로 "배제 원칙"을 다룬다. 특히, 제외선언한 의존성이라고 하더라도 다른 경로로 접근한 의존성에 대해서는 제외가 저용되지 않을 것이다. 예를 들어, 다음과 같이 선언된 starter POM에서는:
```xml
<dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-core</artifactId>
        <version>4.0.5.RELEASE</version>
        <exclusions>
            <exclusion>
                <groupId>commons-logging</groupId>
                <artifactId>commons-logging</artifactId>
            </exclusion>
        </exclusions>
    </dependency>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>4.0.5.RELEASE</version>
    </dependency>
</dependencies>
```

```commons-logging``` jar는 gradle에 의해서 제외되지 않을 것이다. 왜냐하면 ```spring-context (spring-context → spring-core → commons-logging)```에는 ```exclusion``` 요소가 없기 때문이다.

제대로 제외가 적용되는 것을 보장하기 위해 스프링부트 그레들 플러그인은 자동으로 제외 규칙을 추가한다. 모든 제외는 ```spring-boot-dependencies``` POM에 정의되고 나서 "sta
rter" POMs에 대한 묵시적 규칙이 추가될 것이다.

만약 제외규칙이 자동적으로 적용되는 것을 원하지 않는 경우에는 다음처럼 설정할 수 있다:
```
springBoot {
    applyExcludeRules=false
}
```

### 60.4. 실행가능한 jar 와 war 파일 패키징<a name="60.4. 실행가능한 jar 와 war 파일 패키징"></a>
```spring-boot``` 플러그인은 ```bootRepackage``` 태스크를 실행할 경우 자동적으로 압축파일을 재작성한다. 프로젝트를 jar 혹은 war로 빌드할지를 설정 혹은 선언할 수 있다.

실행하려는 메인 클래스는 매니페스트에 ```Main-Class``` 속성을 추가하거나, 구성옵션을 사용하여 지정할 수 있다. 별도로 메인클래스를 선언하지 않아도 플러그인은 클래스에서 ```public static void main(String[] args)```을 탐색할 것이다.

프로젝트 아티팩트를 빌드하고 실행할때, 다음과 같이 입력한다:

```
$ gradle build
$ java -jar build/libs/mymodule-0.0.1-SNAPSHOT.jar
```

실행가능하거나 외부 컨테이너에 배포가능한 war를 빌드하려면, 내장된 컨테이너 의존성을 다음과 같이 "prvidedRuntime" 설정으로 선언해야한다. 예:
```
...
apply plugin: 'war'

war {
    baseName = 'myapp'
    version =  '0.5.0'
}

repositories {
    jcenter()
    maven { url "http://repo.spring.io/libs-snapshot" }
}

configurations {
    providedRuntime
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    providedRuntime("org.springframework.boot:spring-boot-starter-tomcat")
    ...
}
```
> 팁:
배포가능한 war 파일을 어떻게 생성하는지 보다 자세히 알고 싶다면 [75.1. 배포가능한 war 파일 생성](#75.1. 배포가능한 war 파일 생성)을 살펴보기 바란다.

### 60.5. 프로젝트 바로 실행<a name="60.5. 프로젝트 바로 실행"></a>
jar 빌딩 없이 프로젝트를 실행하려면 "bootRun" 태스크를 사용한다:
```
$ gradle bootRun
```

이 실행방법은 동작중인 애플리케이션의 정적 클래스패스 리소스(기본적으로 ```src/main/resources```)를 재적재가능하도록 만들어, 개발시 도움이 된다.
> 팁:
정적 클래스패스 리소스를 재적재가능하도록 만든다는 의미는 ```bootRun```은 ```processResources``` 태스크의 결과물을 사용하지 않는다. 애플리케이션이 ```bootRun```을 사용할 때 애플리케이션은 절차를 거치지 않은 형식의 리소스를 사용한다.

### 60.6. 스프링부트 플러그인 설정<a name="60.6. 스프링부트 플러그인 설정"></a>
그레들 플러그인은 빌드 스크립트 DSL의 부트 플러그인의 전역 설정의 ```springBoot``` 요소를 자동으로 확장한다. 다른 그레들 확장 속성들을 사용하도록 설정한다(설정사항의 목록에 다음과 같이 한다):
```
springBoot {
    backupSource = false
}
```

### 60.7. 리패키징 설정<a name="60.7. 리패키징 설정"></a>
플러그인에 추가된 ```bootRepackage``` 태스크는 다음처럼 바로 설정할 수 있다:
```
bootRepackage {
    mainClass = 'demo.Application'
}
```

가능한 설정사항들은 다음과 같다:
| 이름 | 설명 |
|------|------|
|```enabled```| Boolean flag는 리패키저를 끄는 스위치다(다른 부트 기능을 원할 때 유용하지만 이것 하나만이 아니다) |
| ```mainClass``` |  실행될 메인 클래스를 정의한다. 만약 프로젝트 속성에 ```mainClassName``` 을 정의하지 않았다면 사용되거나, ```mainClassName``` 가 저으이되지 않았다면 적절한 클래스를 탐색한다. "적절한"은 ```main()``` 메소드를 가지고 있는 유일한 클래스를 의미한다(하나 이상을 찾게 되면 실패한다). "run" 태스크(```main``` 속성)에 사용될 메인 클래스를 정의할 수 있으며 "springBoot" 설정을 사용하여 "startScripts"(```mainClassName``` 속성)을 대안으로 사용할 수 있다. |
| ```classifier``` | 원래 (확장이전) 파일명 세그먼트는 원래 위치에 보존되도록, 아카이브에 추가할 수 있다. 기본이 null인 경우 아카이브에 위치가 재보장된다. 기본값은 많은 목적을 위해 편리하지만 다른 프로젝트의 종속성으로 원래의 jar를 사용할 경우, 실행 파일 압축파일을 정의하는 확장 기능을 사용하는 것이 가장 좋다. |
|```withJarTask```| 재포장하는 압축파일을 찾는데 사용되는 이름이나 ```jar``` 작업의 값(```jar``` 유형의 모든 태스크 기본값) |
|```customConfiguration```|내장된 lib 디렉토리에 자주사용되는 맞춤설정의 이름(이를 지정하지 않으면 모든 컴파일 및 런타임 종속성을 얻음) |

### 60.8. 맞춤 그레들 설정으로 리패키징<a name="60.8. 맞춤 그레들 설정으로 리패키징"></a>
때때로 ```compile```, ```runtime``` 그리고 ```provided``` 스코프로부터 기본 의존성들을 패키지하지 않도록 지시할 수 있다. 만약 생성된 실행가능한 jar 파일을 그 자체로 실행할 경우에는 모든 의존성을 파일 안에 포함하고 있어야할 필요가 있다. 그러나 jar 파일을 압축해제하여 메인 클래스를 실행려는 계획이라면 ```CLASSPATH``` 상에 사용가능한 라이브러리들을 사용할 수 있다.  이런 상황에 맞춰 jar 를 리패키징하는 과정에서 의존성을 다르게 설정할 수 있다.

사용자 정의 설정을 사용한다면 ```compile```, ```runtime``` 과 ```provided``` 스코프를 통해서 자동으로 의존성 설정을 비활성화할 수 있다. 사용자 정의 설정은 전역적(```springBoot``` 섹션 안에서)으로 혹은 태스크에 한정지어 정의할 수 있다.

```
task clientJar(type: Jar) {
    appendix = 'client'
    from sourceSets.main.output
    exclude('**/*Something*')
}

task clientBoot(type: BootRepackage, dependsOn: clientJar) {
    withJarTask = clientJar
    customConfiguration = "mycustomconfiguration"
}
```

위의 예에서, 컴파일된 소스로부터 재정의된 파일을 패키징하는 ```clientJar``` jar 태스크를 생성했다. 그리고 ```clientBoot```  라는 BootRepackage 태스크를 생성하고 ```mycustomconfiguration``` 설정과 함께 ```clientJar``` 태스크와 동작하도록 정의했다.

```
configurations {
    mycustomconfiguration.exclude group: 'log4j'
}

dependencies {
    mycustomconfiguration configurations.runtime
}
```

설정configuration이 참조하고 있는 ```BootRepackage```는 일반적인 [Gradle 설정](http://www.gradle.org/docs/current/dsl/org.gradle.api.artifacts.Configuration.html)이다. 앞에서 살펴본 예제에서  ```runtime```에서 파생되고 ```log4j``` 그룹을 제외하는 ```mycustomconfiguration``` 라는 설정을
생성했다. ```clientBoot``` 태스크가 실행되면, 리패키지된 boot jar는 ```log4j``` jar를 제외한 ```runtime``` 의 의존성들을 가지고 있을 것이다.

#### 60.8.1. 설정 사항
설정가능한 사항들은 다움과 같다:

| 이름 | 설명 |
|------|------|
|```mainClass```|실행가능한 압축파일에서 실행할 메인클래스를 정의|
|```providedConfiguration```|제공된 설정의 이름(기본 ```providedRuntime```|
|```backupSource```| 재압축하기 전에 원본 압축파일을 백업 여부 정의(기본 ```true```|
|```customConfiguration```|사용자 정의 설정 이름 |
|```layout```|내부에 어떤 형태로 의존성을 구성할지, 압축 유형을 정의(압축유형을 기반으로 결정)|
|```requiresUnpack```| 의존성 목록(실행시 fat jar 로부터 풀린 "groupId:artifactId"). 아이템들은 여전히 fat jar 안에 압축된 채로 유지되지만, 실행될 때에는 자동으로 압축해제될 것이다.

### 60.9. 그레들 플러그인의 동작방식 이해<a name="60.9. 그레들 플러그인의 동작방식 이해"></a>
```spring-boot```는 그레들 프로젝트에 ```bootRepackage``` 기본태스크를 자동생성한다. ```bootRepackage``` 태스크는 그레들 ```assemble`` 태스크에 의존성을 가지며, 실행시, qualifier가 비어있는 모든 jar 아티팩트를 찾는다(예, 테스트와 소스 jar는 제낀다).

```bootRepackage```는 '모든' 생성된 jar 아티팩트를 찾는데, 그래들 태스크 실행명령에서 중요하다. 대부분의 프로젝트는 하나의 jar 파일을 생성하는 것이 별다른 문제가 되지는 않는다. 그러나, 좀 더 복잡한 프로젝트 설정을 생성할 계획이라면 ``Jar``` 그리고 ```bootRepackage``` 태스크를 사용자정의할 수 있는 기법 몇개가 있다.

만약 프로젝트에서 사용자정의 ```jar```만 생성하고 싶다면 ```jar```와 ```bootRepackage``` 태스크를 간단하게 비활서오하 시킬 수 있다:
```
jar.enabled = false
bootRepackage.enabled = false
```

다른 선택사항으로는 기본 ```bootRepackage``` 태스크가 기본 ```jar``` 태스크하고만 동작하도록 설정하는 것이다:

```
bootRepackage.withJarTask = jar
```

기본 프로젝트 설정으로 기본 ```jar``` 파일을 생성하고 재압축하고, '거기에 더해서' 추가적으로 사용자 정의 jar를 생성하길 원할 수도 있다, ```dependsOn``` 을 사용하여 ```bootRepackage```가 실행되고 난 후 ```bootJars``` 태스크가 실행되도록 연결할 수도 있다:

```
task bootJars
bootJars.dependsOn = [clientBoot1,clientBoot2,clientBoot3]
build.dependsOn(bootJars)
```

앞에서 살펴본 모든 기법들은 이미 생성된 boot jar를 다시 재압축하는 상황을 모면하는데 사용되었다. 재압축Repackaging은 이미 존재하는 boot jar를 훼손하지 않지만 불필요한 의존성이 포함되어 있는 것을 볼 수 있을 것이다.

### 60.10. 그레들을 이용해서 메이븐 레파지토리에 아티팩트 배포<a name="60.10. 그레들을 이용해서 메이븐 레파지토리에 아티팩트 배포"></a>
[60.2. 버전 없이 의존성 정의](#60.2. 버전 없이 의존성 정의)과 메이븐 레파지토리에 아티팩트를 배포하고 싶다면 스프링부트의 의존성 관리 상세를 통해서 메이븐 출간 설정이 필요할 것이다. ```spring-boot-starter-parent``` 를 상속받아 출시 ```poms```의 설정을 할수도 있고 ```spring-boot-dependencies```로부터 의존성 관리를 임포트할 수도 있다. 이 구성의 정확한 세부 사항은 그레들을 어떻게 사용할지 아티팩트를 어떻게 게시할지에 따라 달라진다.

#### 60.10.1. 그레들 설정을 이용한 상속적 의존성 관리 POM 제작<a name="60.10.1. 그레들 설정을 이용한 상속적 의존성 관리 POM 제작"></a>
``` spring-boot-starter-parent```에서 유전된 POM을 생성하는 그레들 설정 예제다. 보다 자세한 정보는 [그레들 사용자 가이드](http://www.gradle.org/docs/current/userguide/userguide.html)를 살펴보기 바란다.

```
uploadArchives {
    repositories {
        mavenDeployer {
            pom {
                project {
                    parent {
                        groupId "org.springframework.boot"
                        artifactId "spring-boot-starter-parent"
                        version "1.2.0.BUILD-SNAPSHOT"
                    }
                }
            }
        }
    }
}
```

#### 60.10.2. 그레들 설정을 이용한 imports 의존성 관리 POM 제작<a name="60.10.2. 그레들 설정을 이용한 imports 의존성 관리 POM 제작"></a>
```spring-boot-dependencies```에 의해 제공되는 의존성 관리를 가져오는 POM을 생성하는 그레들 설정 예제다. 보다 자세한 정보는 [그레들 사용자 가이드](http://www.gradle.org/docs/current/userguide/userguide.html)를 살펴보기 바란다.

```
uploadArchives {
    repositories {
        mavenDeployer {
            pom {
                project {
                    dependencyManagement {
                        dependencies {
                            dependency {
                                groupId "org.springframework.boot"
                                artifactId "spring-boot-dependencies"
                                version "1.2.0.BUILD-SNAPSHOT"
                                type "pom"
                                scope "import"
                            }
                        }
                    }
                }
            }
        }
    }
}
```

## 61. 다른 빌드 지원 시스템 지원
만약 메이븐이나 그레들 이외의 다른 빌드툴을 사용하길 원한다면, 플러그인을 개발해야할 것이다. 실행가능한 jar는 정의된 형식을 따라야하고 압축해제된 폼 안에 포함되어야할 엔트리를 작성해야하기 때문이다(보다 자세한 사항은 부록에 있는 [부록 D. 실행가능한 jar 형식](#D. 실행가능한 jar 형식) 섹션을 살펴보기 바란다).

스프링부트 메이븐과 그레들 플러그인은 실제로 jar를 생성할 때 둘다 ```spring-boot-loader-tools```를 사용하여 만든다. 필요하다면 자유롭게 이 라이브러리를 사용할 수 있다.

### 61.1. 리패키징 아카이브
있는 압축파일을 재압축은 실행가능한 압축파일에  ```org.springframework.boot.loader.tools.Repackager```를 스스로 포함한다. ```Repackager``` 클래스는 존재하는 jar 혹은 war 에 대한 인자를 받는 단독 생성자를 가지고 있다. 사용가능한 두 개의 ```repackage()``` 메서드 중에서 하나를 사용하여 기존 파일을 대체하거나 새로운 곳에 작성한다. 다양한 설정은 리패키저가 실행되기 전에 할 수 있다.

### 61.2. 내포된 라이브러리
재압축되고 있을 때 참조된 의존성 파일들은 ```org.springframework.boot.loader.tools.Libraries``` 인터페이스를 이용한다. 빌드 시스템에 정의된 항목 외에는 ```Libraries``` 구현체를 제공할 수 없다. 

이미 압축파일 안에 라이브러리들을 포함하고 있다면 ```Libraries.NONE```를 사용하면 된다.

### 61.3. 메인 클래스 탐색
메인 클래스를 정의하는데 ```Repackager.setMainClass()```를 사용하지 않았다면, 리패키저는 [ASM](http://asm.ow2.org/)를 이용하여 클래스 파일을 읽고 ```public static void main(String[] args)``` 메서드를 가지고 있는 적절한 클래스를 찾으려고 할 것이다. 대상이 되는 클래스를 한개 이상 찾게 되면 예외를 던진다.

### 61.4. repackage 구현 예제
여기 기본적인 리패키지 예외가 있다.

```
Repackager repackager = new Repackager(sourceJarFile);
repackager.setBackupSource(false);
repackager.repackage(new Libraries() {
    @Override
    public void doWithLibraries(LibraryCallback callback) throws IOException {
        // Build system specific implementation, callback for each dependency
        // callback.library(new Library(nestedFile, LibraryScope.COMPILE));
    }
});
```

## 62. 다음 읽을 거리
빌드툴 플러그인이 어떻게 동작하는지에 흥미가 있다면 깃헙의 [spring-boot-tools](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-tools)모듈을 살펴볼 수 있다. 보다 기술적인 상세정보는 [부록 D. 실행가능한 jar 형식](#D. 실행가능한 jar 형식)을 살펴보기 바란다.

특정 빌드와 관련된 질문이 있는 경우에는 ['어떻게How-to' 가이드](#'어떻게How-to' 가이드) 를 살펴보라.

# IX. '어떻게How-to' 가이드<a name="'어떻게How-to' 가이드"></a>
혹시 우리가 대비하지 못한 부분들에서 문제들이 발생한다면 [스택오버플로우](http://stackoverflow.com/tags/spring-boot)에서 이미 누군가가 작성한 답변을 확인할 수도 있다: 이곳은 새로운 질문을 올리기에도 좋은 곳이다(```spring-boot``` 태그를 사용하자).

# 63. 스프링부트 애플리케이션
### 63.1. 자동설정 문제해결
스프링부트 자동설정은 '적절한 것을 한다'를 최고가치로 여기고 있지만 가끔 실패하고 왜 그런지 말하기 어려울 때가 있다.

그런 때에 스프링부트 `ApplicationContext`에  `AutoConfigurationReport`이 유용하다. `DEBUG` 로깅출력을 했을 때 볼 수 있다. `spring-boot-actuator`를 사용하면 `autoconfig` 엔드포인트를 통해서 JSON으로된 결과를 받을 수 있다. 애플리케이션을 디버그하고 실행시 스프링부트가 제공하는 추가적인 기능들(그리고 할 수 없는 것들)은 무엇이 있는지 살펴보자.

보다 많은 질문은 소스코드와 Javadoc을 살펴보면 답을 찾을 수 있을 것이다. 몇가지 룰이 있다면:
* `*AutoConfiguration` 클래스를 찾아보고 그 소스코드를 읽어보라, `@Conditional*` 애노테이션이 사용된 부분들을 찾아보고 그 기능이 활성화 되기 위한 조건이 무엇인지 살펴본다. 커맨드라인에서 `--debug` 을 추가하거나 시스템 프로퍼티 `-Ddebug`를 통해 애플리케이션에서 만들어진 자동설정 결정사항들을 콘솔 로그로 볼 수 있다. 액츄에이터 앱이 실행되고 있다면 `autoconfig` 엔드포인트(`/autoconfig` 혹은 JMX equivalent)를 통해서 같은 정보를 볼 수 있다.
* `@ConfigurationProperties`(예, [`ServerProperties`](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/web/ServerProperties.java)) 와 가능한 외부 설정 옵션들을 살펴본다. `@ConfigurationProperties`는 `name` 속성은 외부 프로퍼티즈들의 접두어로 사용한다. `ServerProperties`는 `prefix="server"`이고 그 설정 속성들은 `server.port`, `server.address` 등이 있다. 실행중인 액추에이터 앱은 `configprops` 엔드포인트에서 찾아볼 수 있다.
* 명시적 `Environment`에서 구성값을 추출하여 `RelaxedEnvironment`의 사용을 찾는다. 접두사로 종종 사용된다.
* `@Value` 애노테이션을 살펴보면 `Environment`에 바로 연결된다. 이 일부 느슨한 결합을 허용하지만 `RelaxedEnvironment` 접근보다는 OS 환경변수에 대한 접근 유연성이 부족하다.
* `@ConditionalOnExpression` 애노테이션을 찾아 SpEL 을 표현식에 대한 응답으로 온오프 기능 전환, `Environment`으로부터 위치변환자를 통해 확인한다. 


### 63.2. 시작 전 ```Environment``` 혹은 ```ApplicationContext``` 변경
`SpringApplication`는 `ApplicationListeners`와 `ApplicationContextInitializers`르 가지고 있으며 이를 사용하여 컨텍스트나 환경에 대한 사용자설정을 허용한다. 스프링부트는 내부의 `META-INF/spring.factories`를 사용하여 다양한 사용자설정을 적재한다. 추가하는 방법은 다음과 같다:

* `SpringApplication`가 실행되기 전에 `addListeners`와 `addInitializers` 메서드에 구현한다.
* 선언적으로 `context.initializer.classes` 혹은 `context.listener.classes` 설정을 정의한다.
* `META-INF/spring.factories` 을 선언하고 jar로 만들어 모든 애플리케이션에 라이브러리로 사용한다.

`SpringApplication`은 리스너들에 `ApplicationEvents`를 보낸다(컨텍스트가 생성되기도 전에), 그리고 `ApplicationContext`를 발표되는 이벤트에 대한 리스너로 등록한다. 스프링부트 기능 관련 항목 중에서 [22.4. "애플리케이션 이벤트와 리스너"](#22.4. 애플리케이션 이벤트와 리스너)를 보라.

### 63.3. ```ApplicationContext``` 계층 빌드(부모 혹은 루트 컨텍스트 추가)
`ApplicationBuilder` 클래스를 사용하여 부모/자식 `ApplicationContext` 계층을 생성한다. 이와 관련된 사항은 '스프링부트 기능' 항목의 [22.3. 플루언트 빌더 API](#22.3. 플루언트 빌더 API)를 살펴보라.

### 63.4. non-web 애플리케이션 생성
모든 스프링 애플리케이션이 웹 애플리케이션(웹 서비스)이어야 하는 건 아니다. 뿐만 아니라 스프링 애플리케이션을 구동하여 인프라를 설정하고 `main` 메서드를 실행하고 싶다면 스프링부트의 `SpringApplication` 기능을 통해 쉽게할 수 있다. `SpringApplication`은 웹 애플리케이션이 필요한지에 따라 `ApplicationContext` 클래스를 변경한다. 첫번째 해야할 것은 클래스패스 상에서 서블릿 API 의존성들을 모두 제거해야 한다. 만약 그렇게 할 수 없다면(예를 들어, 같은 코드로 2개의 애플리케이션을 실행하고 있다면) `SpringApplication.setWebEnvironment(false)` 설정하거나, `applicationContextClass` 프로퍼티를 설정해야 한다(Java API나 외부 프로퍼티즈를 통해서). 비즈니스 로직을 실행하려면 `CommandLineRunner`를 구현하고 `@Bean` 정의를 컨텍스트에서 삭제한다.

## 64. 속성 및 설정
### 64.1. 스프링애플리케이션의 설정 확장<a name="64.1. 스프링애플리케이션의 설정 확장"></a>
`SpringApplication` 은 애플리케이션이 생성될 때 행위를 변경할 수 있는 Java API 로 사용할 수 있는 속성들(기본 setters사용)을 가지고 있다. 혹은 `spring.main.*` 속성을 사용하여 외부적으로 설정할 수 있다. 예를 들어, `application.properties`에 다음과 같이 설정한다면:

```
spring.main.web_environment=false
spring.main.show_banner=false
```

이렇게 설정하면, 시작시 스프링부트 배너가 출력되지 않고, 애플리케이션은 웹 애플리케이션이 아닐 것이다.

> 노트: 
예제에 있는 구분자로 언더스코어(`_`) 혹은 대시(`-`)를 속성 이름에 사용하는 것도 허용한다.

### 64.2. 애플리케이션의 외부 속성 위치 변경<a name="64.2. 애플리케이션의 외부 속성 위치 변경"></a>
서로 다른 소스코드로부터 기본 속성들을 정의된 순서에 따라 Spring `Environement` 에 추가할 수 있다('스프링 부트 기능' 섹션의 (23. 외부설정)[#23. 외부설정]을 보라).

인자를 통해 넘기는 것이 좋은 방법이며 `@PropertySource` 애노테이션을 애플리케이션 소스에 추가하여 변경할 수 있다. 클래스는 `SpringApplication` 정적 관례적인 메서드에 전달하고 `@PropertySrouce`를 가지고 있는지 검사한 후에 `setSources()`를 사용하여 추가한다, 그렇게 하고나면, 그 속성은 초기에 `ApplicationContext` 생명주기의 모든 단계의 `Environment`에 추가된다. 이 방법으로 추가된 속성은 기본설정으로 추가된 것보다 우선순위를 가지지만, 시스템 속성, 환경변수 혹은 명령행보다는 낮은 순위를 가지게 된다.

또한 시스템 속성을 변경할 수 있는 방법을 제공한다:
* `spring.config.name`(`SPRING_CONFIG_NAME`), 파일명은 `application`으로 구성
* `spring.config.location`(`SPRING_CONFIG_LOCATION`)는 파일이 적재되는 위치를 지정한다(예, 클래스패스 리소스 혹은 URL). 분리된 `Environment` 속성 소스는 이 문서를 통해서 설정할 수 있으며, 시스템 속성, 환경변수 혹은 명령행에서 정의된 속성들을 덮어쓰기 할 수 있다.

어떤 환경설정을 하던지 스프링부트는 항상 `application.properties`를 읽어온다고 앞에서 이야기 했다. YAML은 `.yml` 확장자를 가진 파일을 사용하는 경우도 기본적으로 목록에 추가된다. 

보다 자세한 사항은 [`ConfigFileApplicationListener`](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/context/config/ConfigFileApplicationListener.java)을 살펴보기 바란다.

### 64.3. '간략한' 커맨드라인 인자 사용<a name="'간략한' 커맨드라인 인자 사용"></a>
몇몇 이들은 명령행에서 `--server.port=9000` 대신에 `--port=9000`을 사용하여 설정하길 원하는 이들이 있을 것이다. `application.properties`에서 위치변환자를 사용하여 쉽게 설정할 수 있다, 예
```
server.port=${port:8080}
```

> 팁:
`spring-boot-starter-parent` POM을 상속받았다면, `maven-resources-plugins`의 기본 필터토큰은 스프링 스타일의 위치변환자를 통해 충돌을 예방하며 `${*}`으로 변경할 수 있다(예, `@maven.token@` 대신에 `${maven.token}`). 만약 `application.properties`를 바로 메이븐 필터링을 활성화하고 있다면, [다른 구분자](http://maven.apache.org/plugins/maven-resources-plugin/resources-mojo.html#delimiters)를 사용하여 기본 필터 토큰을 변경할 수도 있다.

> 노트:
Heroku와 Cloud Foundry 와 같은 PaaS 환경에서는 특정 작업 포트가 지정된 경우가 있다, 이 두가지 플랫폼에서는 `PORT` 환경변수가 있어 자동설정되며 스프링은 `Environment` 속성을 대문자 동의어로 연결할 수 있다.

### 64.4. 외부 속성을 YAML로 정의<a name="64.4. 외부 속성을 YAML로 정의"></a>
YAML은 JSON 타입의 상위설정이며 계층형 형태의 외부속성을 위한 매우 편리한 문법을 제공한다. 예

```yml
spring:
    application:
        name: cruncher
    datasource:
        driverClassName: com.mysql.jdbc.Driver
        url: jdbc:mysql://localhost/test
server:
    port: 9000
```

`application.yml` 이란 파일을 만들고 루트 클래스패스에 위치시키고, `snakeyaml` 의존성을 추가한다(메이븐 의존성 `org.yaml:snakeyaml`은, 이미 `spring-boot-starter` 를 사용하여 포함하고 있다). YAML 파일은 Java `Map<String,Object>` 형태로 파싱하고, 스프링부트는 평평한 지도 1단계 깊이로 구분된 키로 구성는데, 몇몇 이들은 자바에서 `Properties` 를 사용하는 것을 선호하는 이들도 있다.

다음의 예는 위에서 YAML에 작성한 내용을  `application.properties` 파일로 작성한 것이다.

```
spring.application.name=cruncher
spring.datasource.driverClassName=com.mysql.jdbc.Driver
spring.datasource.url=jdbc:mysql://localhost/test
server.port=9000
```

YAML에 대한 보다 자세한 정보는 '스프링부트 기능' 섹션에 [23.5. Properties 대신 YAML 사용](#23.5. Properties 대신 YAML 사용)를 살펴보라.

### 64.5. 활성 스프링 프로파일 설정<a name="64.5. 활성 스프링 프로파일 설정"></a>
스프링 `Environment`는 이것을 위한 API를 가지고 있으며, 시스템 프로파일(`spring.profils.active`) 를 OS 환경 변수(`SPRING_PROFILES_ACVIE`)을 설정할 수 있다. 예로, 애플리케이션을 실행할 때 `-D` 인자와 함께 실행(메인 클래스 혹은 jar 아카이브 전에 실행해야 한다):

```
$ java -jar -Dspring.profiles.active=production demo-0.0.1-SNAPSHOT.jar
```

혹은 스프링부트에서 `application.properties` 를 통해 활성 프로파일이 설정할 수도 있다:

```
spring.profiles.active=production
```

이 방법으로 설정된 값은 시스템 속성 혹은 환경변수 설정을 대체한다, 그러나 `SpringApplicationBuilder.profiles()` 메서드에 의한 것은 아니다. 그래서 Java API를 사용하면 기본값을 변경하지 않고 프로파일을 인자로 사용할 수 있다. 

보다 자세한 내용은 '스프링부트 기능' 섹션에 [24. 프로파일](#24. 프로파일)을 살펴보기 바란다. 

### 64.6. 환경 의존적 설정 변경<a name="64.6. 환경 의존적 설정 변경"></a>
YAML 파일은 `---` 줄을 기준으로 분리된 문서들로 구성된다, 그리고 각 문서는 독립된 평평한 맵의 형태로 파싱된다.

만약 YAML 문서에 `spring.profiles` 키가 포함되어 있다면, 프로파일 값(프로파일의 콤마로 분리된 목록)은 스프링 `Environment.acceptsProfiles()`에 설정되고 활성화된 문서의 프로파일에 병합된다(혹은 그렇지 않을 수도 있다).
> 역자주: **프로파일이 설정되지 않은 문서의 내용**은 **프로파일이 설정된 문서의 내용**이 덮어씌여지고 프로파일 설정된 문서의 내용에 없는 부분은 병합된다.

예:
```yaml
server:
    port: 9000
---

spring:
    profiles: development
server:
    port: 9001

---

spring:
    profiles: production
server:
    port: 0
```

이 예제에서 기본 포트는 9000번이다, 그러나 스프링 프로파일 'development'가 활성화되면 포트는 9001이 활성화되고, 'production' 이 활성화되면 0이 된다.

YAML 문서는 마주친 순서대로 우선순위를 가지고 병합된다(그래서 최근 값이 이전의 것들을 덮어쓴다).

같은 방법을 프로퍼티즈 파일에서 사용하기 위해서는 `application-${profile}.properties` 를 사용해서 프로파일-설정 값을 설정해야 한다.

### 64.7. 외부 속성들의 빌트인 항목 살펴보기<a name="64.7. 외부 속성들의 빌트인 항목 살펴보기"></a>
스프링부트는 애플리케이션이 실행될 때 `application.properties` (or `.yml`) 확장 속성들과 연결(혹은 다른 위치들을 포함)된다. 단독 위치에 있는 모든 지원가능한 속성을 다 사용하는 것은 아니다(기술적으로 불가능). 왜냐하면 클래스패스상에 추가된 jar 파일들에서 제공받기 때문이다.

실행중인 애플리케이션은 `configprops` 엔드포인트 액추에이터 기능을 통해 `@ConfigurationProperties`을 통해 연결가능한 속성들과 연결된 속성들을 모두 보여준다.

부록에 있는 [application.properties](#A. 일반적인 애플리케이션 속성) 예제에는 스프링부트에서 지원하는 거의 모든 속성들의 목록이 있다. `@ConfigurationProperties`와 `@Value` 애노테이션이 선언된 소스코드를 탐색하여 정의돈 목록은 `RelaxedEnvironment` 에 의해 사용된다.

## 65. 내장형 서블릿 컨테이너<a name="65. 내장형 서블릿 컨테이너"></a>
### 65.1. Servlet, Filter 혹은 ServletContextListener 를 애플리케이션에 추가
Servlet, Filter, ServletContextListener 그리고 서블릿 스펙을 지원하는 다른 리스너들은 애플리케이션에서 `@Bean` 정의로 추가할 수 있다. eager 초기화 때문에 너무 많은 빈이 등록되지 않도록 매우 조심해야하는데 컨테이너는 애플리케이션 생명주기에서 매우 초기에 설치되기 때문이다(예, `DataSource` 혹은 JPA 설정을 이 녀석들에게 의존하는 것은 좋은 생각이 아니다). 초기화 대신에 처음 사용할 때에는 느슨한 초기화를 하는 것이 좋다.

`Filter`와 `Servlets`의 경우 `FilterRegisterBean` 혹은 `ServletREgisterationBean` 을 사용하여 초기화 파라메터와 연결할 수 있다. 

### 65.2. HTTP 포트 변경
단독실행 애플리케이션의 메인 HTTP 포트는 `8080`이다, 그러나 `server.port` 를 사용하여 설정할 수 있다(예를 들어, `application.properties` 혹은 시스템 속성을 통해). `Environment`값의 관련된 연결 덕분에 또한 `SERVER_PORT`를 사용할 수 있다(예, OS 환경 변수).

`WebApplicationContext`를 만들 때, `server.port=-1`(테스트에 유용)를 사용하여 HTTP 엔드포인트를 완벽하게 전환할 수 있다.()

### 65.3. HTTP 포트를 지정하지 않고 무작위로 사용<a name="65.3. HTTP 포트를 지정하지 않고 무작위로 사용"></a>
`server.port=0`을 사용하면 포트를 탐색하여 사용하지 않는 포트를 사용한다.

### 65.4. 실행시 HTTP Port 살펴보기
실행중인 서버의 로그출력물이나 `EmbeddedServletContainer`을 통한 `EmbeddedWebApplicationContext` 에 접근할 수 있다. 최적의 방법은 `ApplicationListener<EmbeddedServletContainerInitializedEvent>` 타입의 `@Bean`을 초기화 과정에 추가하고 퍼블리싱된 이벤트들을 컨테이너쪽으로 끌어오는 것이다.

`server.port=0`으로 설정학고 `@IntegrationTests`를 하면 실제 포트(`local`)는 `@Value`를 통해 주입받는 유용한 실습이 가능하다. 예를 들자면:

```java
@RunWith(SpringJUnit4ClassRunner.class)
@SpringApplicationConfiguration(classes = SampleDataJpaApplication.class)
@WebAppConfiguration
@IntegrationTest("server.port:0")
public class CityRepositoryIntegrationTests {

    @Autowired
    EmbeddedWebApplicationContext server;

    @Value("${local.server.port}")
    int port;

    // ...

}
```

### 65.5. SSL 설정<a name="65.5. SSL 설정"></a>
SSL 은 `application.properties` 혹은 `application.yml`에 `server.ssl.*` 속성을 통해 다양한 설정들을 정의할 수 있다. 예를 들자면:
```
server.port = 8443
server.ssl.key-store = classpath:keystore.jks
server.ssl.key-store-password = secret
server.ssl.key-password = another-secret
```

지원하는 속성들에 대한 보다 자세한 사항들은 [Ssl](http://github.com/spring-projects/spring-boot/tree/master/spring-boot/src/main/java/org/springframework/boot/context/embedded/Ssl.java) 을 살펴보자.

> 노트:
톰캣이 요구하는 key store(사용하려는 신뢰가능한 저장체)는 파일시스템을 통해 바로 접근이 가능해야 한다, 예를 들어, jar 파일을 통해서 읽어올 수는 없다.

### 65.6. 톰캣 설정<a name="65.6. 톰캣 설정"></a>
`@ConfigurationProperties`(`ServerProperties`는 여기서 주속성 중 하나)에 관한 조언들은 [64.7. 외부 속성들의 빌트인 항목 살펴보기](#64.7. 외부 속성들의 빌트인 항목 살펴보기)을 통해 따를 수 있다. 거기에 더해 `EmbeddedServletContainerCustomizer` 과 다양한 톰캣을위한 `*Customizers`을 추가할 수 있다. 톰캣 API는 `TomcatEmbeddedServletContainerFactory`에 접근할 수 있는 막강한 기능을 부여하여 변경할 수 있는 다양한 수단을 제공한다. 혹은 `TomcatEmbeddedServletContainerFactory`를 직접 추가하여 선택사항을 초기화할 수 있다.

### 65.7. 톰캣의 다중커넥터 활성화<a name="65.7. 톰캣의 다중커넥터 활성화"></a>
`TomcatEmbeddedServletContainerFactory`에 `org.apache.catalina.connector.Connector` 인터페이스를 구현한 다양한 커넥터를 허용한다. 예를 들어, HTTP and HTTPS 커넥터.

```java

```

### 65.8. 톰캣을 프론트엔드 프록시 서버로 사용<a name="65.8. 톰캣을 프론트엔드 프록시 서버로 사용"></a>
스프링부트는 톰캣의 `RemoteIpValve`가 활성화 되어 있다면 자동으로 설정한다. 이 설정은 표준 `x-forwarded-for` 와 `x-forwarded-proto`헤더를 투명하게 사용할 수 있도록 하여 거의 모든 프론트엔드 프록시 서버에 추가할 수 있다. 밸브는 하나 혹은 양쪽 속성이 비어있지 않다면 설정을 변환할 수 있다(관례적인 값은 대부분 프록시를 사용하며 하나를 설정하면 다른 것은 자동으로 설정된다).

```
server.tomcat.remote_ip_header=x-forwarded-for
server.tomcat.protocol_header=x-forwarded-proto
``` 

프록시로 다른 헤더를 사용한다면 `application.properties`  항목을 추가하여 밸브 설정을 사용자가 정의할 수 있다.

```
server.tomcat.remote_ip_header=x-your-remote-ip-header
server.tomcat.protocol_header=x-your-protocol-header
```

또한 밸브는 신뢰할 수 있는 내부 프록시 맞춤에 기본 정규 표현식을 사용한다. 기본적으로 IP주소는 `10/8`, `192.168/16`, `169.254/16` and `127/8`을 신뢰한다. 밸브의 설정값은 `application.properties`에 항목을 추가하여 변경할 수 있다.

```
server.tomcat.internal_proxies=192\\.168\\.\\d{1,3}\\.\\d{1,3}
```

> 노트: 
이중 백슬러시는 설저응ㄹ 위해서 프로퍼티즈를 사용할 때만 필요하다. YAML을 사용하고 있다면 `192\.168\.\d{1,3}\.\d{1,3}` 다음과 같이 싱글 백슬러시를 사용하면 같은 효과를 볼 수 있다.

대안으로, `TomcatEmbeddedServletContainerFactory` 빈을 추가하고 `RemoteIpValve` 설정을 조절하면 제어를 완료할 수도 있다.

### 65.9. 톰캣 대신 제티 사용<a name="65.9. 톰캣 대신 제티 사용"></a>
스프링부트 스타터(`spring-boot-starter-web` 일부)는 기본 내장 컨테이너로 톰캣을 사용한다. 필요하다면 그 의존성을 제외하고 대신 제티를 포함시킬 수 있다. 스프링부트는 톰캣과 제티에 관한 의존성을 기본제공하여 스타터를 분리하여 이 과정을 쉽게 가능하도록 돕고 있다.

메이븐 예:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
    <exclusions>
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
        </exclusion>
    </exclusions>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-jetty</artifactId>
</dependency>
```

그레들 예:
```gradle
configurations {
    compile.exclude module: "spring-boot-starter-tomcat"
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web:1.2.0.BUILD-SNAPSHOT")
    compile("org.springframework.boot:spring-boot-starter-jetty:1.2.0.BUILD-SNAPSHOT")
    // ...
}
```

### 65.10. 제티 설정<a name="65.10. 제티 설정"></a>
`@ConfigurationProperties`에 관한 내용은 [64.7. 외부 속성들의 빌트인 항목 살펴보기](#64.7. 외부 속성들의 빌트인 항목 살펴보기)을 따르면 도움이 될 것이다(`ServerProperties`도 여기에 있다), 그리고 `EmbeddedServletContainerCustomizer`를 살펴보라. 제티 API는 매우 풍부한데 `JettyEmbeddedServletContainerFactory`를 통해 접근가능하며 다양한 방법으로 변경할 수 있다. 혹은 `JettyEmbeddedServletContainerFactory`를 추가하여 초기화시킬 수 있다.

### 65.11. 톰캣 대신 언더토우Undertow 사용<a name="65.11. 톰캣 대신 언더토우Undertow 사용"></a>
[65.9. 톰캣 대신 제티 사용](#65.9. 톰캣 대신 제티 사용)와 매우 유사하게 톰캣 대신 언더토우를 사용할 수 있다. 톰캣 의존성을 제외시키고 언더토우 스타터를 대신 포함시키면 된다.

메이븐 예:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
    <exclusions>
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
        </exclusion>
    </exclusions>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-undertow</artifactId>
</dependency>
```

그레들 예:
```
configurations {
    compile.exclude module: "spring-boot-starter-tomcat"
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web:1.2.0.BUILD-SNAPSHOT")
    compile("org.springframework.boot:spring-boot-starter-undertow:1.2.0.BUILD-SNAPSHOT")
    // ...
}
```

### 65.12. 언더토우 설정<a name="65.12. 언더토우 설정"></a>
`@ConfigurationProperties`에 관한 내용은 [64.7. 외부 속성들의 빌트인 항목 살펴보기](#64.7. 외부 속성들의 빌트인 항목 살펴보기)을 따르면 도움이 될 것이다(`ServerProperties`도 여기에 있다), 그리고 `EmbeddedServletContainerCustomizer`를 살펴보라. 필요하다면 언더토우의 설정은 `UndertowBuilderCustomizer`를 사용하여 변경할 수 있으며 `UndertowEmbeddedServletContainerFactory` 에 접근가능하다. 혹은 `UndertowEmbeddedServletContainerFactory` 구현하여 초기화할 수 있다.


### 65.13. 톰캣 7 사용<a name="65.13. 톰캣 7 사용"></a>
톰캣 7도 스프링부트에서 동작한다, 그러나 기본은 톰캣 8을 사용한다. 톰캣 8을 사용할 수 없다면(예를 들어, 자바 1.6을 사용한다거나) 톰캣 7과 서블릿 API 3.0을 참조하는 클래스 패스를 변경해야 한다.

만약 스타터 poms와 parents를 사용하고 있다면 버전 속성만 변경하면 된다. 다음의 간단한 예를 보자:

```xml
<properties>
    <tomcat.version>7.0.56</tomcat.version>
    <servlet-api.version>3.0.1</servlet-api.version>
</properties>
<dependencies>
    ...
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>
    ...
</dependencies>
```

### 65.14. 제티 8 사용<a name="65.14. 제티 8 사용"></a>
스프링부트에서는 제티8을 사용할 수 있지만, 기본적으로는 제티 9을 사용한다. 만약 제티 9을 사용할 수 없다면(예를 들어, 자바 1.6을 사용한다거나) 제티 8과 서블릿 API 3.0을 참조하는 클래스패스를 변경하면 된다. 추가적으로 제티의 웹소켓관련 의존성을 제외시켜야 한다.

만약 스타터 poms와 parent를 사용중이라면 웹소켓 요구사항을 제외시키고 버전 속성을 변경하면 된다. 다음의 간단한 예를 보자:

```xml
<properties>
    <jetty.version>8.1.15.v20140411</jetty.version>
    <jetty-jsp.version>2.2.0.v201112011158</jetty-jsp.version>
    <servlet-api.version>3.0.1</servlet-api.version>
</properties>
<dependencies>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
        <exclusions>
            <exclusion>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-starter-tomcat</artifactId>
            </exclusion>
        </exclusions>
    </dependency>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-jetty</artifactId>
        <exclusions>
            <exclusion>
                <groupId>org.eclipse.jetty.websocket</groupId>
                <artifactId>*</artifactId>
            </exclusion>
        </exclusions>
    </dependency>
</dependencies>
```
### 65.15. `@ServerEndpoint`를 사용해서 웹소켓 엔드포인트 생성<a name="65.15. `@ServerEndpoint`를 사용해서 웹소켓 엔드포인트 생성"></a>
스프링부트 애플리케이션에서 `@ServerEndpoint`와 내장 컨테이너를 사용하고 있다면 `ServerEndpointExporter` `@Bean`은 단독으로 선언해야 한다:

```java
@Bean
public ServerEndpointExporter serverEndpointExporter() {
    return new ServerEndpointExporter();
}
```

이 빈은 다른 `@ServerEndPoint` 애노테이션을 사용한 빈과 함께 웹소켓 컨테이너에 등록된다. 단독 서블릿 컨테이너가 배포될 때 서블릿 컨테이너 초기화의 역할을 수행하며 `ServerEndpointExporter` 빈은 필요하지 않다.

## 66. 스프링 MVC
### 66.1. JSON REST 서비스 작성
### 66.2. XML REST 서비스 작성
### 66.3. Jackson ObjectMapper 변경
### 66.4. ```@ResponseBody``` 렌더링 변경
### 66.5. ```Multipart``` 파일 업로드 제어
### 66.6. Spring MVC ```DispatcherServlet``` 끄기
### 66.7. 기본 MVC 설정 끄기
### 66.8. ViewResolver 변경

## 67. 로깅

스프링부트는 의존 라이브러리들이 가진 ```commons-logging``` API를 제외하곤 로깅 라이브러리를 자유롭게 선택할 수 있다. [Logback](http://logback.qos.ch/)을 사용하기를 원한다면 먼저 Logback을 포함하고, ```commons-logging```을 연결하면 된다. 가장 간단한 방법은 ```spring-boot-starter-logging```이 내부에 포함되어 있는 Starter pom을 사용하는 것이다. 로깅 라이브러리에 의존하고 있기에 ```spring-boot-starter-web``` 만 있으면 된다. 메이븐에서는 아래와 같이 사용할 수 있다. 

```
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

스프링부트는 추상화된 ```LoggingSystem```을 가지고 있으며, 클래스패스를 기준으로 설정을 시도한다. 만약 Loback이 가능할 경우 첫번째로 선택된다.

```application.properties``` 파일에 "logging.level"로 시작하는 로거와 레벨을 추가하는 것만으로 로깅을 시작할 수 있다. 

```
logging.level.org.springframework.web: DEBUG
logging.level.org.hibernate: ERROR
```

또한 "logging.file"을 사용하여 로깅파일의 위치(콘솔에도 출력)를 지정하여 줄 수 있다.

조금 더 상세한 설정을 위해서는 각 구현체가 요구하는 설정양식을 사용하여야 한다. 기본적으로 스프링부트는 설정파일을 기본 경로에서 찾으며(Logback의 경우 ```classpath:logback.xml```), 이 경로는 "logging.config" 속성을 통해 변경하여줄 수 있다.

### 67.1. 로깅을 위한 Logback 설정

```logback.xml```을 classpath의 root에 추가하여 설정값을 지정하여줄 수 있다. 스프링 부트는 기본 설정을 제공하고 있으며, 로깅레벨을 변경할 필요가 있을 경우 아래와 같이 설정이 가능하다.

```
<?xml version="1.0" encoding="UTF-8"?>
<configuration>
    <include resource="org/springframework/boot/logging/logback/base.xml"/>
    <logger name="org.springframework.web" level="DEBUG"/>
</configuration>
```

spring-boot jar내부의 기본 ```logback.xml```에서는 ```LoggingSystem```이 제공해주는 유용한 시스템 변수들을 찾을 수 있을 것이다.

- ${PID} : 현재 프로세스ID.
- ${LOG_FILE} : 직접 지정한 ```logging.file```의 위치.
- ${LOG_PATH} : 직접 지정한 ```logging.path```의 위치(로그파일이 저장되는 위치).

스프링부트는 콘솔(파일은 제외)에 출력되는 로그의 ANSI색상을 지정할 수 있다. 관련 기본설정은 ```base.xml```에서 확인할 수 있다.

만약 Groovy가 클래스패스에 존재하면 ```logback.groovy```파일을 사용하여 설정을 정의할 수 있다.(존재하는 경우 기본 설정값도 적용됨)


### 67.2. 로깅을 위한 Log4j 설정

스프링부트는 [Log4j](http://logging.apache.org/log4j/1.2), [Log4j 2](http://logging.apache.org/log4j/2.x)가 클래스패스에 존재할 경우에 설정할 수 있도록 지원한다. 만약 Starter pom을 사용하여 의존관계를 지정하였다면 반드시 Logback을 제거한뒤 사용할 버전의 Log4j를 추가하여야 한다. 만약 Starter pom을 사용하지 않을 경우에는 Log4j에 해당하는 ```commons-logging```(최소한) 제공하여 주어야 한다.

Log4j를 적용하는 간단한 방법은 Starter pom을 사용(exclude구문이 복잡하게 나타나긴 하지만)하는 것이다.

```
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter</artifactId>
    <exclusions>
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-logging</artifactId>
        </exclusion>
    </exclusions>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-log4j</artifactId>
</dependency>
```

Log4j 2를 사용한다면 ```spring-boot-starter-log4j2```를 ```spring-boot-starter-log4j```대신 사용하라.

> 팁 : Log4j Staeter를 공통로깅을 한군데 모으는데 사용하기를 원한다면 (예를들어, 톰캣이 `java.util.logging`을 사용하지만, Log4j 또는 Log4j 2의 설정으로 로깅을 할 경우) Actuator Log4j 또는 Log4j 2 의 샘플에서 어떻게 동작하는지 살펴볼 수 있다.

## 68. <a name="데이터 접근">데이터 접근</a>

### 68.1. <a name="데이터소스 설정">데이터소스 설정</a>

```DataSource```를 ```@Bean```으로 정의하기만 하면 데이터소스 설정이 완료된다. 스프링 부트는 빌더 클래스 ```DataSourceBuilder```를 제공하며 클래스패스에서 정의된 값을 기준으로 만들거나, 또는```Environment```에 정의된 값을 사용하여 만들 수 있다:

```
@Bean
@ConfigurationProperties(prefix="datasource.mine")
public DataSource dataSource() {
    return new FancyDataSource();
}

datasource.mine.jdbcUrl=jdbc:h2:mem:mydb
datasource.mine.user=sa
datasource.mine.poolSize=30
```

보다 자세한 내용은 '스프링부트 기능'섹션의 [28.1. 데이터베이스 설정](#데이터베이스 설정) 섹션이나, [DataSourceAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jdbc/DataSourceAutoConfiguration.java)클래스를 참조하여라.

### 68.2. <a name="복수 데이터소스 설정">복수 데이터소스 설정</a>

하나 이상의 데이터소스를 사용하기 위한 방법은 위와 동일하다.  이 경우 데이터소스에 ```@Primary```를 표기하면 JDBC나 JPA에서 기본으로 사용될 데이터소스가 무엇인지를 표기하여 줄 수 있다.

```
@Bean
@Primary
@ConfigurationProperties(prefix="datasource.primary")
public DataSource primaryDataSource() {
    return DataSourceBuilder.create().build();
}

@Bean
@ConfigurationProperties(prefix="datasource.secondary")
public DataSource secondaryDataSource() {
    return DataSourceBuilder.create().build();
}
```

### 68.3. <a name="스프링 데이터 레파지토리 사용">스프링 데이터 레파지토리 사용</a>

스프링 데이터는 ```@Repository```인터페이스를 사용하여 다양하게 구현할 수 있다. 스프링부트는 ```@EnableAutoConfiguration``` 클래스를 기준으로 동일한 (또는 그 아래) 패키지에 존재하는 ```@Repository```클래스들을 다룰 수 있습니다.

스프링 부트를 사용하여 작성하는 애플리케이션의 클래스패스에는 그에 맞는 의존관계가 설정되어야 한다.(JPA를 사용한다면 ```spring-boot-starter-data-jpa```를 몽고를 사용한다면```spring-boot-starter-data-mongodb```가 필요하다.)

스프링 부트는 ```@EnableAutoConfiguration```을 기준으로 ```@Repository```의 설정값을 추측한다. 상세한 설정이 필요하다면 JPA의 설정이 담긴 ```@EnableJpaRepositories```같은 걸 사용하는 것처럼 설정이 필요하다.

### 68.4. <a name="스프링 설정으로 부터 @Entity 정의 분리">스프링 설정으로 부터 ```@Entity``` 정의 분리</a>

스프링 부트는 ```@EnableAutoConfiguration```을 기준으로 ```@Entity```의 설정값을 추측한다. 상세한 설정이 필요하다면 아래와 같이 ```@EntityScan```을 사용하도록 하자 : 

```
@Configuration
@EnableAutoConfiguration
@EntityScan(basePackageClasses=City.class)
public class Application {

    //...

}
```

### 68.5. <a name="JPA 속성 설정">JPA 속성 설정</a>

스프링 데이터 JPA는 벤더에 의존적인 설정 옵션들을 지원하며(예를 들어 SQL Logging) 스프링부트에서는 이에 더해 몇몇 하이버네이트의 설정을 지원한다. 주로 사용되는 옵션들을 다음과 같이 설정할 수 있다 : 

```
spring.jpa.hibernate.ddl-auto: create-drop
spring.jpa.hibernate.naming_strategy: org.hibernate.cfg.ImprovedNamingStrategy
spring.jpa.database: H2
spring.jpa.show-sql: true
```

```ddl-auto```의 설정값은 특정기술에 따라 기본값이 다르게 설정된다. 임베디드 데이터베이스일 경우에는 ```create-drop```로 설정되며, 아닐경우에는 ```none```으로 설정된다. 또한  ```spring.jpa.properties.*```로 설정된 값들은 EntityManagerFactory가 생성될때 JPA의 속성으로 설정된다.(설정키 앞의 spring.jpa.properties는 무시된다.)

더욱 자세한 내용은 [HibernateJpaAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/orm/jpa/HibernateJpaAutoConfiguration.java)과 [JpaBaseConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/orm/jpa/JpaBaseConfiguration.java)을 참조하여라.

### 68.6. <a name="EntityManagerFactory 변경">```EntityManagerFactory``` 변경</a>

```EntityManagerFactory```의 모든 상세한 설정이 필요하다면, ‘entityManagerFactory'의 ```@Bean```이 필요하다. 스프링부트의 자동설정은 해당 타입의 빈여부에 따라 설정이 변경된다.

### 68.7. <a name="복수 엔티티매니저 사용">복수 엔티티매니저 사용</a>


기본으로 설정된 ```EntityManagerFactory```가 정상적으로 동작하더라도 새로운 엔티티매니저 팩토리를 만들 경우에 기본 설정이 무시되므로, 아래와 같이 둘다 함께 빈을 설정하여야 한다 : 


```
// 데이터소스 설정이 이미 존재한다고 가정한다.

@Bean
public LocalContainerEntityManagerFactoryBean customerEntityManagerFactory(
        EntityManagerFactoryBuilder builder) {
    return builder
            .dataSource(customerDataSource())
            .packages(Customer.class)
            .persistenceUnit("customers")
            .build();
}

@Bean
public LocalContainerEntityManagerFactoryBean orderEntityManagerFactory(
        EntityManagerFactoryBuilder builder) {
    return builder
            .dataSource(orderDataSource())
            .packages(Order.class)
            .persistenceUnit("orders")
            .build();
}
```

위의 설정은 거의 완벽하게 동작하지만, ```EntityManager```에 대한 ```TransactionManager``` 설정이 포함되어있지 않다. 두 엔티티 매니저상단에 ```@Primary```을 추가하여 기본값을 추가할 수 있으며, 그 외의 엔티티매니저는 각 사용할 클래스에서 명시적으로  설정하여 사용할 수 있다. 또는 JTA의 트랜잭션을 사용하여 둘을 동시에 사용할수도 있다.

### 68.8. <a name="전통적인 persistence.xml 사용">전통적인 ```persistence.xml``` 사용</a>

스프링은 JPA의 설정에서 XML을 요구하지 않으며 이는 스프링 부트도 마찬가지이다. 만약 ```persistence.xml```를 사용하기를 원할 경우, ```LocalEntityManagerFactoryBean```의 타입을 빈(이 빈의 id는 ‘entityManagerFactory’)으로 선언하고, persistence unit의 이름으로 설정하여라.

스프링 부트에 설정된 기본 설정은 [JpaBaseConfiguration](https://github.com/spring-projects/spring-boot/blob/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/orm/jpa/JpaBaseConfiguration.java)클래스를 확인하여라.

### 68.9. <a name="스프링데이터 JPA와 몽고 레파지토리 사용">스프링데이터 JPA와 몽고 레파지토리 사용</a>

스프링 Data JPA와 스프링 Data Mongo 둘 모두 자동으로 Repository를 설정해준다. 만약 클래스 패스에 의존관계가 존재한다면, 스프링 부트에서 어떤 Repository가 필요한지(또는 둘 모두)를 설정해 주어야 한다. 가장 명시적인 방법은 Spring Data에서 기본으로 제공하는 ```@Enable*Repositories```을 ```Repository```상단에 추가하는 것이다.(*에는 'Jpa'와 'Mongo'둘 다 사용할 수 있다.)

설정파일의 키값 ```spring.data.*.repositories.enabled``` 을 사용하면 자동설정여부를 켜거나 끌 수 있다. 기존의 Mongo Repsitory가 아닌 자동 설정된 ```MongoTemplate``` 를 사용하는 경우에 유용하게 사용할 수 있을 것이다.

동일한 문제점과 기능이 다른 자동 설정되는 Spring Data에도(Elasticsearch, Solr) 에도 적용된다.각 변경되는 어노테이션과 플래그들이 다르므로 유의하여 사용하도록 하자.

## 69. 데이터베이스 초기화<a name="69. 데이터베이스 초기화"></a>
SQL 데이터베이스는 어떤 스택을 사용하느냐에 따라서 다른 방법들로 초기화할 수 있다. 혹은 각 단계별로 데이터베이스에 메뉴얼적으로 처리하는 방법도 있다.

### 69.1. JPA 사용하여 데이터베이스 초기화<a name="69.1. JPA 사용하여 데이터베이스 초기화"></a>
JPA는 DDL 생성 기능을 가지고 있으며 데이터베이스와는 달리 기동이 시작되는 순간에 설정할 수 있다. 이부분은 두가지 확장 속성을 통해 제어가능하다:
* `spring.jpa.generate-ddl` (boolean) 는 기능을 켜거나 끌 수 있으며 벤더에 의존적이지 않다.
* `spring.jpa.hibernate.ddl-auto` (enum) 는 하이버네이트 기능으로 보다 합리적인 방법으로 행동을 제어할 수 있다. 자세한 내용은 다음과 같다.

### 69.2. Hibernate를 사용하여 데이터베이스 초기화<a name="69.2. Hibernate를 사용하여 데이터베이스 초기화"></a>
`spring.jpa.hibernate.ddl-auto` 에 설정가능한 표준 하이버네이트 속성값은 `none`, `validate`, `update`, `create-drop` 이 있다. 스프링부트이 선택하는 기본값은 데이터베이스가 내장형인 경우(기본 `create-drop`)와 그렇지 않은 경우(기본 `none`)으로 생각해볼 수 있다. 내장형 데이터베이스는 `Connection` 유형을 탐색하여 `hsqldb`, `h2` 그리고 `derby`이면 내장형, 그 이외에는 내장형이 아니라고 판단한다. 인-메모리를 **'실제'** 데이터베이스로 변경할 때 새로운 플랫폼 안에 테이블과 데이터가 존재할 것이라고 추측하지 않도록 주의해야 한다. 명시적으로 `ddl-auto` 을 설정하거나, 다른 데이터베이스 초기화 기작을 사용하는 것이 좋다.

추가적으로, `import.sql` 파일명을 가진 파일이 루트 클래스패스에 있다면 시동시 실행될 것이다. 이것은 잘 관리만 한다면 데모와 테스트를 위해서 매우 유용하지만, 출시제품의 경우에는 없기를 바라는 경우도 있을 것이다. 이것은 하이버네이트의 기능이다(스프링은 아무것도 하지 않는다).

### 69.3. Spring JDBC를 사용하여 데이터베이스 초기화<a name="69.3. Spring JDBC를 사용하여 데이터베이스 초기화"></a>
스프링 JDBC는 `DataSource` 초기화 기능을 가지고 있다. 스프링부트는 기본적으로 그 기능을 활성화하고 있으며 표준 위치에 있는 `schema.sql`과 `data.sql`로부터 SQL을 읽어온다(클래스패스 루트). 추가적으로 스프링부트는 `schema-${platform}.sql` 그리고 `data-${platform}.sql` 파일을 읽을 것이다(파일들이 존재한다면), `platform`의 값은 `spring.datasource.platform` 값이며, 그 값들은 데이터베이스 벤더 이름들(`hsqldb`, `h2`, `oracle`, `mysql`, `postgresql` 등 )중에서 선택할 수 있다. 스프링부트는 스프링 JDBC 초기화에 대해서 '빠른 실패'를 기본으로 하고 있다. 그래서 애플리케이션 시작시 스크립트로 인해 예외가 생기면 시동에 실패한다. 스크립트 위치는 `spring.datasource.schema` 그리고 `spring.datasource.data` 를 설정하여 변경할 수 있으며 `spring.datasource.initialize=false` 속성을 설정하면 동작하지 않는다.

`spring.datasource.continueOnError=true` 설정을 하면 '빠른 실패' 를 비활성화할 수 있다. 이것은 애플리케이션 개발이 완료되고 배포되는 시점에 유용하다. 스크립트는 가난한 남자의 이주‘poor man’s migrations’처럼 동작하여 입력실패는 데이터가 이미 존재한다는 의미기 때문에, 애플리케이션이 실행되거나 인스턴스로 동작할 때 방지할 필요가 없는 경우에 사용하면 된다.

JPA app(하이버네이트를 함께 사용하는 경우)에서 `schema.sql`를 사용하고자 할 때 `ddl-auto=create-drop` 사항을 선택하여 하이버네이트가 같은 테이블을 생성하려고 시도하면서 에러가 발생할 수 있다. 이 상황을 피하기 위해서는 `ddl-auto`를 명시적으로 `""` 혹은 `"none"`을 설정하면 된다. `ddl-auto=create-drop`를 사용하지 않으면 항상 `data.sql`을 통해 새로운 데이터를 초기화할 것이다.

### 69.4. 스프링 배치 데이터베이스 초기화<a name="69.4. 스프링 배치 데이터베이스 초기화"></a>
스프링배치를 사용하면 대부분의 인기있는 데이터베이스 플랫폼을 위한 SQL 초기화 스크립트를 사전에 패키징할 수 있다. 스프링부트는 데이터베이스 타입을 탐색하여 그에 적합한 스크립트를 실행할 수 있으며 '빠른 실패'를 비활성화 처리할 수 있다(에러는 로그로 출력되지만 애플리케이션이 시작되는 것을 차단하지는 않는다). 이런 이유로 스크립트는 신뢰할 수 있는 것으로 알려져 있으며, 일반적으로 버그가 포함되어 있지 않기 때문에 오차가 무시할 수 있을 정도이며 이를 무시하는 스크립트는 상호불변적이다. 명시적으로 `spring.batch.initializer.enabled=false`를 사용하여 초기화를 끌 수 있다.

### 69.5. 고차원 데이터베이스 마이그레이션 도구 사용<a name="69.5. 고차원 데이터베이스 마이그레이션 도구 사용"></a>
스프링부트는 [Flyway](http://flywaydb.org/)(SQL-기반) 그리고 [Liquibase](http://www.liquibase.org/)(XML) 과 같은 높은수준의 마이그레이션 도구를 사용할 수 있다. Flyway를 추천하는데 그 이유는 눈으로 읽기 쉽고, 플랫폼 의존성을 크게 요구하지 않기 때문이다: 보틍 플랫폼과 긴밀한 것이 하나이상 필요하다.

#### 69.5.1. 시작시 Flyway 실행하여 데이터베이스 마이그레이션<a name="69.5.1. 시작시 Flyway 실행하여 데이터베이스 마이그레이션"></a>
시동시 Flyway 데이터베이스 마이그레이션 도구를 자동으로 실행하기 위해서는, `org.flywaydb:flyway-core`가 클래스패스에 추가되어야 한다.

마이그레이션을 위한 스크립트는 ` V<VERSION>__<NAME>.sql` 형태여야 한다(그리고 `<VERSION>`은 `'1'` 혹은 `'2_'` 형태로 구분된다). 기본 동작폴더는 `classpath:db/migration` 이지만 `flyway.location`(목록)을 사용하여 변경할 수 있다. `flyway-core`에 있는 Flyway 클래스들을 보다 자세히 살펴보면 `schemas` 와 기타 등등을 상세히 설정할 수 있다. 추가적으로 스프링부트는 [FlywayProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/flyway/FlywayProperties.java)를 통해서 세부적으로 설정할 수 있으며 마이그레이션을 비활성화하거나 위치 점검을 끌 수 있다.

기본적으로 Flyway는 마이그레이션을 사용한다면 컨텍스트의 `(@Primary) DataSource`와 자동연결된다. 만약 다른 `DataSource`를 사용하려한다면 `@Bean` 그 위에 `@FlywayDataSource`를 표시하면 된다 - 두 개의 데이터소스를 사용하길 원한다면 하나에는 `@Primary` 를 표시해야한다는 것을 기억해두자. 혹은 flyway에서 제공하는 `DataSource`를 사용하려 한다면 `flyway`를 설정하면 된다. 확장 프로퍼티즈에 [`url`,`user`,`password`]가 있다.

[Flyway 예제](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-flyway)를 보면 어떻게 설정할 수 있는지 살펴볼 수 있다.

#### 69.5.2. 시작시 Liquibase를 실행하여 데이터베이스 마이그레이션<a name="69.5.2. 시작시 Liquibase를 실행하여 데이터베이스 마이그레이션"></a>

시동시 Liquibase 데이터베이스 마이그레이션이 자동으로 실행되게 하려면, `org.liquibase:liquibase-core`를 클래스패스에 추가해야 한다.

마스터 변경로그는 `db/changelog/db.changelog-master.yaml`을 읽어오지만 `liquibase.change-log`를 사용하도록 설정할 수 있다. [LiquibaseProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/liquibase/LiquibaseProperties.java) 를 보면 컨텍스트, 기본 스키마 등의 설정을 할 수 있는 것들을 살펴볼 수 있다.

[Liquibase 예제](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-liquibase)를 살펴보면 어떻게 설정할 수 있을지 살펴볼 수 있다.

## 70. 배치 애플리케이션
### 70.1. 시작시 스프링 배치 작업 실행

스프링 배치 자동설정은 컨텐스트와 관련된 클래스에 `@EnableBatchProcessing`(스프링 배치로 부터)를 추가하면 활성화된다.

**모든** `Jobs`는 기본적으로 애플리케이션 컨텍스트가 시작될 때 실행된다(보다 자세한 사항은 [`JobLauncherCommandLineRunner`](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/batch/JobLauncherCommandLineRunner.java)을 살펴보자).  `spring.batch.job.names`을 통해 특정 작업 또는 작업들로 좁힐 수 있다(콤마로 구분되는 작업 이름 패턴).

만약 애플리케이션 컨텍스트에 `JobRegistry`가 포함된 경우 컨텍스트로부터 자동연결된 것을 대신하여 `spring.batch.job.names` 의 작업들이 등록된다. 이것은 여러 작업이 자식 컨텍스트에 정의고 중앙에 등록된 더욱 복잡한 시스템의 일반적인 패턴이다.

보다 자세한 사항들은 [BatchAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/batch/BatchAutoConfiguration.java)와 [@EnableBatchProcessing](https://github.com/spring-projects/spring-batch/blob/master/spring-batch-core/src/main/java/org/springframework/batch/core/configuration/annotation/EnableBatchProcessing.java)를 살펴보기 바란다.

## 71. 액츄에이터Actuator
### 71.1. 액츄에이터 엔드포인트의 주소 혹은 HTTP 포트 변경
단독실행중인 애플리케이션의 액추에이터 HTTP 포트는 기본적으로 메인 HTTP port와 동일한 것을 사용한다. 애플리케이션 액추에이터 접속 포트를 변경하려고 한다면 `management.port` 확장 속성을 다르게 설정하면 된다. 다른 네트워크 주소로 접근하도록 하고자 할 경우(관리를 위한 내부 네트워크를 가지고 있거나 사용자 애플리케이션 중 외부의 하나) `management.address`에 서버에 연결할 수 있는 검증된 IP 주소를 설정할 수 있다.

보다 자세한 사항은 [ManagementServerProperties](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-actuator/src/main/java/org/springframework/boot/actuate/autoconfigure/ManagementServerProperties.java) 소스코드를 살펴보거나 '출시 준비 기능' 세션의 [41.3. 관리 서버포트 변경](#41.3. 관리 서버포트 변경)를 살펴보라.

### 71.2. 'whitelabel' 오류 페이지 변경
스프링부트는 서버 에러가 발생했을 때 클라이언트 브라우저에서 볼 수 있는 'whitelable'에러페이지가 설치되어 있다(클라이언트에 JSON으로

## 72. 시큐리티
### 72.1. 스프링부트 시큐리티 설정 끄기<a name="72.1. 스프링부트 시큐리티 설정 끄기"></a>
`@Configuration` 와 `@EnableWebSecurity`가 선언된 곳이면 어디서든지 스프링부트의 기본 웹앱 보안설정을 끌 수 있다. `security.*` 에 기본설정들은 변경할 수 있다([`SecurityProperties`](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/security/SecurityProperties.java) 에서 보다 자세한 설정가능항목들을 볼 수 있다) 그리고 [일반적인 애플리케이션 속성](#A. 일반적인 애플리케이션 속성) 부분 중에서 `SECURITY` 항목에 보다 자세한 설정들이 있다.

### 72.2. `AuthenticationManager`를 변경하고 사용자 계정 추가

`AuthenticationManager` 타입의 `@Bean`을 제공한다면 기본설정의 것은 생성되지 않는다, 그러면 스프링 시큐리티의 가능한 모든 기능들을 설정해야 한다(예, [다양한 인증 선택항목들](http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#jc-authentication))

스프링 시큐리티는 또한 편리한 `AuthenticationManagerBuilder`을 제공하여 일반적인 선택항목들과 함께 `AuthenticationManager` 를 빌드할 수 있도록 해준다. 웹앱에서 사용시 권장하는 방법은 `WebSecurityConfigurerAdapter` void 메서드에 추가하는 방법이다, 예:

```java
@Configuration
public class SecurityConfiguration extends WebSecurityConfigurerAdapter {

    @Autowired
    public void configureGlobal(AuthenticationManagerBuilder auth) throws Exception {
            auth.inMemoryAuthentication()
                .withUser("barry").password("password").roles("USER"); // ... etc.
    }

    // ... other stuff for application security

}
```

여기에 nested 클래스혹은 단독실행 클래스(인스턴스화 순위에 영향을 끼치는 다른 `@Bean`이 섞이지 않은)를 추가하면 가장 좋은 결과를 얻을 것이다. [security web 예제](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-web-secure)는 따라하기 용이한 형틀이다.

만약 구체적인 이슈에 대한 경험이 있다면(예를 들어, JDBC 혹은 JPA를 사용하여 사용자 상세정보UserDetails를 저장) `GlobalAuthenticationConfigurerAdapter` 안에서 `AuthenticationManagerBuilder`를 콜백으로 추출할 수있다(인증매니저가 다른 곳에서 필요로 하기 전에 `init()` 메서드가 먼저 호출된다). 예,
```java
@Configuration
public class AuthenticationManagerConfiguration extends

    GlobalAuthenticationConfigurerAdapter {
    @Override
    public void init(AuthenticationManagerBuilder auth) {
        auth.inMemoryAuthentication() // ... etc.
    }

}
```

## 73. 핫스와핑
### 73.1. 정적컨텐츠 다시 읽기
### 73.2. 컨테이너 재시작없이 타임리프Thymeleaf 템플렛 다시 읽기
### 73.3. 컨테이너 재시작없이 프리마크FreeMarker 템플렛 다시 읽기
### 73.4. 컨테이너 재시작없이 그루비Groovy 템플렛 다시 읽기
### 73.5. 컨테이너 재시작없이 벨로시티Velocity 템플렛 다시 읽기
### 73.6. 컨테이너 재시작없이 자바 클래스 다시 읽기
#### 73.6.1. 메이븐을 이용한 Spring Loaded 설정
#### 73.6.2. 그레들과 IntelliJ를 이용한 Spring Loaded 설정

## 74. 빌드
### 74.1. 메이븐으로 의존성 버전 변경
### 74.2. 메이븐으로 실행가능한 JAR 생성
### 74.3. 추가적인 실행가능한 JAR 생성
### 74.4. 실행가능한 jar 동작에 필요한 지정된 라이브러리 추출
### 74.5. 배제를 통한 실행할 수 없는 JAR 생성
### 74.6. 메이븐을 이용해서 스프링부트 애플리케이션 원격 디버그 시작
### 74.7. 그레들을 이용해서 스프링부트 애플리케이션 원격 디버그 시작
### 74.8. 앤트를 이용해서 실행가능한 아카이브 빌드<a name="앤트를 이용해서 실행가능한 아카이브 빌드"></a>

## 75. 전통적 배포<a name="75. 전통적 배포"></a>
### 75.1. 배포가능한 war 파일 생성<a name="75.1. 배포가능한 war 파일 생성"></a>
### 75.2. 오래된 서블릿 컨테이너에 배포가능한 war 파일 생성<a name="75.2. 오래된 서블릿 컨테이너에 배포가능한 war 파일 생성"></a>
### 75.3. 기존의 애플리케이션을 스프링부트로 변환<a name="75.3. 기존의 애플리케이션을 스프링부트로 변환"></a>
### 75.4. 웹로직을 위한 war 배포<a name="75.4. 웹로직을 위한 war 배포"></a>
### 75.5. 오래된(Servlet 2.5) 컨테이너에 war 배포<a name="75.5. 오래된(Servlet 2.5) 컨테이너에 war 배포"></a>

# X. 부록<a name="X. 부록"></a>
## A. 일반적인 애플리케이션 속성<a name="A. 일반적인 애플리케이션 속성"></a>
```application.properties/application.yml``` 파일 혹은 커맨드라인 스위치를 통해서 다양한 속성들을 정의할 수 있다. 이번 세션에서는 공통적인 스프링부트의 속성목록과 그 속성을 사용하는 연관성있는 클래스를 제공한다.

> 노트:
이 목록을 완전히 고려해서는 안되는데 그 이유는 클래스패스에 추가된 jar 파일에서도 속성을 가져올 수 있기 때문이다. 또한 필요한 경우에는 자신의 속성을 정의하여 사용가능하다.

> 위험:
이 예제 파일은 안내를 목적으로 한다. 애플리케이션에 복사해서 붙여넣지 마라. 필요한 속성만 사용하자.

```
# ===================================================================
# COMMON SPRING BOOT PROPERTIES
#
# This sample file is provided as a guideline. Do NOT copy it in its
# entirety to your own application.               ^^^
# ===================================================================

# ----------------------------------------
# CORE PROPERTIES
# ----------------------------------------

# SPRING CONFIG (ConfigFileApplicationListener)
spring.config.name= # 설정파일명 (기본은 'application')
spring.config.location= # 설정파일 위치

# PROFILES
spring.profiles.active= # comma list of active profiles
spring.profiles.include= # unconditionally activate the specified comma separated profiles

# APPLICATION SETTINGS (SpringApplication)
spring.main.sources=
spring.main.web-environment= # 기본에 의한 탐색
spring.main.show-banner=true
spring.main....= # 보다 자세한 속성은 클래스를 확인

# LOGGING
logging.path=/var/logs
logging.file=myapp.log
logging.config= # 로깅설정파일 위치 (기본 classpath:logback.xml for logback)
logging.level.*= # 로거 레벨, e.g. "logging.level.org.springframework=DEBUG" (TRACE, DEBUG, INFO, WARN, ERROR, FATAL, OFF)

# IDENTITY (ContextIdApplicationContextInitializer)
spring.application.name=
spring.application.index=

# EMBEDDED SERVER CONFIGURATION (ServerProperties)
server.port=8080
server.address= # 별도의 NIC와 연동
server.session-timeout= # 초단위의 세션 타임아웃
server.context-parameters.*= # 서블릿 컨텍스트 초기화 파라메터, 예. server.context-parameters.a=alpha
server.context-path= # 컨텍스트 경로, 기본  '/'
server.servlet-path= # 서블릿경로, 기본 '/'
server.ssl.client-auth= # 원하거나 필요한 경우
server.ssl.key-alias=
server.ssl.ciphers= # SSL ciphers 지원
server.ssl.key-password=
server.ssl.key-store=
server.ssl.key-store-password=
server.ssl.key-store-provider=
server.ssl.key-store-type=
server.ssl.protocol=TLS
server.ssl.trust-store=
server.ssl.trust-store-password=
server.ssl.trust-store-provider=
server.ssl.trust-store-type=
server.tomcat.access-log-pattern= # 접근기록 로그패턴
server.tomcat.access-log-enabled=false # 접근기록 활성화여부
server.tomcat.internal-proxies=10\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|\\
        192\\.168\\.\\d{1,3}\\.\\d{1,3}|\\
        169\\.254\\.\\d{1,3}\\.\\d{1,3}|\\
        127\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3} # 신뢰가능한 IP 주소에 대한 정규표현식
server.tomcat.protocol-header=x-forwarded-proto # front end proxy forward header
server.tomcat.port-header= # front end proxy port header
server.tomcat.remote-ip-header=x-forwarded-for
server.tomcat.basedir=/tmp # base dir (usually not needed, defaults to tmp)
server.tomcat.background-processor-delay=30; # in seconds
server.tomcat.max-http-header-size= # maximum size in bytes of the HTTP message header
server.tomcat.max-threads = 0 # number of threads in protocol handler
server.tomcat.uri-encoding = UTF-8 # character encoding to use for URL decoding

# SPRING MVC (WebMvcProperties)
spring.mvc.locale= # 지역 설정, 예. en_UK
spring.mvc.date-format= # 날짜형식 설정, 예. dd/MM/yyyy
spring.mvc.message-codes-resolver-format= # PREFIX_ERROR_CODE / POSTFIX_ERROR_CODE
spring.mvc.ignore-default-model-on-redirect=true # If the the content of the "default" model should be ignored redirects / 리다이렉트시 모델의 컨텐츠를 무시한다는 뜻
spring.view.prefix= # MVC view prefix
spring.view.suffix= # ... and suffix
spring.resources.cache-period= # 브라우저에 캐시 타임아웃을 헤더로 전달하는 주기
spring.resources.add-mappings=true # if default mappings should be added

# HTTP encoding (HttpEncodingProperties)
spring.http.encoding.charset=UTF-8 # HTTP 요청/응답 인코딩 설정
spring.http.encoding.enabled=true # HTTP 인코딩 지원여부
spring.http.encoding.force=true # 인코딩 강제처리 설정

# JACKSON (JacksonProperties)
spring.jackson.date-format= # 데이터형식 문자열 (예. yyyy-MM-dd HH:mm:ss), 혹은 날짜 형식 클래스의 완전한 경로 (e.g. com.fasterxml.jackson.databind.util.ISO8601DateFormat)
spring.jackson.property-naming-strategy= # One of the constants on Jackson's PropertyNamingStrategy (e.g. CAMEL_CASE_TO_LOWER_CASE_WITH_UNDERSCORES) or PropertyNamingStrategy 클래스의 하위클래스 완전한 경로
spring.jackson.deserialization.*= # see Jackson's DeserializationFeature
spring.jackson.generator.*= # see Jackson's JsonGenerator.Feature
spring.jackson.mapper.*= # see Jackson's MapperFeature
spring.jackson.parser.*= # see Jackson's JsonParser.Feature
spring.jackson.serialization.*= # see Jackson's SerializationFeature

# THYMELEAF (ThymeleafAutoConfiguration)
spring.thymeleaf.check-template-location=true
spring.thymeleaf.prefix=classpath:/templates/
spring.thymeleaf.excluded-view-names= # 구현에서 제외될 뷰 이름을 콤마(,)로 구분하여 목록정리
spring.thymeleaf.view-names= # comma-separated list of view names that can be resolved
spring.thymeleaf.suffix=.html
spring.thymeleaf.mode=HTML5
spring.thymeleaf.encoding=UTF-8
spring.thymeleaf.content-type=text/html # ;charset=<encoding> 를 추가
spring.thymeleaf.cache=true # 캐시처리하지 않을경우 false 설정

# FREEMARKER (FreeMarkerAutoConfiguration)
spring.freemarker.allow-request-override=false
spring.freemarker.cache=true
spring.freemarker.check-template-location=true
spring.freemarker.charset=UTF-8
spring.freemarker.content-type=text/html
spring.freemarker.expose-request-attributes=false
spring.freemarker.expose-session-attributes=false
spring.freemarker.expose-spring-macro-helpers=false
spring.freemarker.prefix=
spring.freemarker.request-context-attribute=
spring.freemarker.settings.*=
spring.freemarker.suffix=.ftl
spring.freemarker.template-loader-path=classpath:/templates/ # comma-separated list
spring.freemarker.view-names= # whitelist of view names that can be resolved

# GROOVY TEMPLATES (GroovyTemplateAutoConfiguration)
spring.groovy.template.cache=true
spring.groovy.template.charset=UTF-8
spring.groovy.template.configuration.*= # See Groovy's TemplateConfiguration
spring.groovy.template.content-type=text/html
spring.groovy.template.prefix=classpath:/templates/
spring.groovy.template.suffix=.tpl
spring.groovy.template.view-names= # whitelist of view names that can be resolved

# VELOCITY TEMPLATES (VelocityAutoConfiguration)
spring.velocity.allow-request-override=false
spring.velocity.cache=true
spring.velocity.check-template-location=true
spring.velocity.charset=UTF-8
spring.velocity.content-type=text/html
spring.velocity.date-tool-attribute=
spring.velocity.expose-request-attributes=false
spring.velocity.expose-session-attributes=false
spring.velocity.expose-spring-macro-helpers=false
spring.velocity.number-tool-attribute=
spring.velocity.prefer-file-system-access=true # prefer file system access for template loading
spring.velocity.prefix=
spring.velocity.properties.*=
spring.velocity.request-context-attribute=
spring.velocity.resource-loader-path=classpath:/templates/
spring.velocity.suffix=.vm
spring.velocity.toolbox-config-location= # velocity Toolbox config location, for example "/WEB-INF/toolbox.xml"
spring.velocity.view-names= # whitelist of view names that can be resolved

# JERSEY (JerseyProperties)
spring.jersey.type=servlet # servlet or filter
spring.jersey.init= # init params
spring.jersey.filter.order=

# INTERNATIONALIZATION (MessageSourceAutoConfiguration)
spring.messages.basename=messages
spring.messages.cache-seconds=-1
spring.messages.encoding=UTF-8


# SECURITY (SecurityProperties)
security.user.name=user # login username
security.user.password= # login password
security.user.role=USER # role assigned to the user
security.require-ssl=false # advanced settings ...
security.enable-csrf=false
security.basic.enabled=true
security.basic.realm=Spring
security.basic.path= # /**
security.filter-order=0
security.headers.xss=false
security.headers.cache=false
security.headers.frame=false
security.headers.content-type=false
security.headers.hsts=all # none / domain / all
security.sessions=stateless # always / never / if_required / stateless
security.ignored=false

# DATASOURCE (DataSourceAutoConfiguration & DataSourceProperties)
spring.datasource.name= # name of the data source
spring.datasource.initialize=true # populate using data.sql
spring.datasource.schema= # a schema (DDL) script resource reference
spring.datasource.data= # a data (DML) script resource reference
spring.datasource.sql-script-encoding= # a charset for reading SQL scripts
spring.datasource.platform= # the platform to use in the schema resource (schema-${platform}.sql)
spring.datasource.continue-on-error=false # continue even if can't be initialized
spring.datasource.separator=; # statement separator in SQL initialization scripts
spring.datasource.driver-class-name= # JDBC Settings...
spring.datasource.url=
spring.datasource.username=
spring.datasource.password=
spring.datasource.jndi-name # For JNDI lookup (class, url, username & password are ignored when set)
spring.datasource.max-active=100 # Advanced configuration...
spring.datasource.max-idle=8
spring.datasource.min-idle=8
spring.datasource.initial-size=10
spring.datasource.validation-query=
spring.datasource.test-on-borrow=false
spring.datasource.test-on-return=false
spring.datasource.test-while-idle=
spring.datasource.time-between-eviction-runs-millis=
spring.datasource.min-evictable-idle-time-millis=
spring.datasource.max-wait=
spring.datasource.jmx-enabled=false # Export JMX MBeans (if supported)

# DATASOURCE (PersistenceExceptionTranslationAutoConfiguration
spring.dao.exceptiontranslation.enabled=true

# MONGODB (MongoProperties)
spring.data.mongodb.host= # the db host
spring.data.mongodb.port=27017 # the connection port (defaults to 27107)
spring.data.mongodb.uri=mongodb://localhost/test # connection URL
spring.data.mongodb.database=
spring.data.mongodb.authentication-database=
spring.data.mongodb.grid-fs-database=
spring.data.mongodb.username=
spring.data.mongodb.password=
spring.data.mongodb.repositories.enabled=true # if spring data repository support is enabled

# JPA (JpaBaseConfiguration, HibernateJpaAutoConfiguration)
spring.jpa.properties.*= # properties to set on the JPA connection
spring.jpa.open-in-view=true
spring.jpa.show-sql=true
spring.jpa.database-platform=
spring.jpa.database=
spring.jpa.generate-ddl=false # ignored by Hibernate, might be useful for other vendors
spring.jpa.hibernate.naming-strategy= # naming classname
spring.jpa.hibernate.ddl-auto= # defaults to create-drop for embedded dbs
spring.data.jpa.repositories.enabled=true # if spring data repository support is enabled

# JTA (JtaAutoConfiguration)
spring.jta.log-dir= # transaction log dir
spring.jta.*= # technology specific configuration

# SOLR (SolrProperties})
spring.data.solr.host=http://127.0.0.1:8983/solr
spring.data.solr.zk-host=
spring.data.solr.repositories.enabled=true # if spring data repository support is enabled

# ELASTICSEARCH (ElasticsearchProperties})
spring.data.elasticsearch.cluster-name= # The cluster name (defaults to elasticsearch)
spring.data.elasticsearch.cluster-nodes= # The address(es) of the server node (comma-separated; if not specified starts a client node)
spring.data.elasticsearch.repositories.enabled=true # if spring data repository support is enabled

# DATA RESET (RepositoryRestConfiguration})
spring.data.rest.base-uri= # base URI against which the exporter should calculate its links

# FLYWAY (FlywayProperties)
flyway.check-location=false # check that migration scripts location exists
flyway.locations=classpath:db/migration # locations of migrations scripts
flyway.schemas= # schemas to update
flyway.init-version= 1 # version to start migration
flyway.init-sqls= # SQL statements to execute to initialize a connection immediately after obtaining it
flyway.sql-migration-prefix=V
flyway.sql-migration-suffix=.sql
flyway.enabled=true
flyway.url= # JDBC url if you want Flyway to create its own DataSource
flyway.user= # JDBC username if you want Flyway to create its own DataSource
flyway.password= # JDBC password if you want Flyway to create its own DataSource

# LIQUIBASE (LiquibaseProperties)
liquibase.change-log=classpath:/db/changelog/db.changelog-master.yaml
liquibase.check-change-log-location=true # check the change log location exists
liquibase.contexts= # runtime contexts to use
liquibase.default-schema= # default database schema to use
liquibase.drop-first=false
liquibase.enabled=true
liquibase.url= # specific JDBC url (if not set the default datasource is used)
liquibase.user= # user name for liquibase.url
liquibase.password= # password for liquibase.url

# JMX
spring.jmx.enabled=true # Expose MBeans from Spring

# RABBIT (RabbitProperties)
spring.rabbitmq.host= # connection host
spring.rabbitmq.port= # connection port
spring.rabbitmq.addresses= # connection addresses (e.g. myhost:9999,otherhost:1111)
spring.rabbitmq.username= # login user
spring.rabbitmq.password= # login password
spring.rabbitmq.virtual-host=
spring.rabbitmq.dynamic=

# REDIS (RedisProperties)
spring.redis.database= # database name
spring.redis.host=localhost # server host
spring.redis.password= # server password
spring.redis.port=6379 # connection port
spring.redis.pool.max-idle=8 # pool settings ...
spring.redis.pool.min-idle=0
spring.redis.pool.max-active=8
spring.redis.pool.max-wait=-1
spring.redis.sentinel.master= # name of Redis server
spring.redis.sentinel.nodes= # comma-separated list of host:port pairs

# ACTIVEMQ (ActiveMQProperties)
spring.activemq.broker-url=tcp://localhost:61616 # connection URL
spring.activemq.user=
spring.activemq.password=
spring.activemq.in-memory=true # broker kind to create if no broker-url is specified
spring.activemq.pooled=false

# HornetQ (HornetQProperties)
spring.hornetq.mode= # connection mode (native, embedded)
spring.hornetq.host=localhost # hornetQ host (native mode)
spring.hornetq.port=5445 # hornetQ port (native mode)
spring.hornetq.embedded.enabled=true # if the embedded server is enabled (needs hornetq-jms-server.jar)
spring.hornetq.embedded.server-id= # auto-generated id of the embedded server (integer)
spring.hornetq.embedded.persistent=false # message persistence
spring.hornetq.embedded.data-directory= # location of data content (when persistence is enabled)
spring.hornetq.embedded.queues= # comma-separated queues to create on startup
spring.hornetq.embedded.topics= # comma-separated topics to create on startup
spring.hornetq.embedded.cluster-password= # customer password (randomly generated by default)

# JMS (JmsProperties)
spring.jms.jndi-name= # JNDI location of a JMS ConnectionFactory
spring.jms.pub-sub-domain= # false for queue (default), true for topic

# Email (MailProperties)
spring.mail.host=smtp.acme.org # mail server host
spring.mail.port= # mail server port
spring.mail.username=
spring.mail.password=
spring.mail.default-encoding=UTF-8 # encoding to use for MimeMessages
spring.mail.properties.*= # properties to set on the JavaMail session

# SPRING BATCH (BatchDatabaseInitializer)
spring.batch.job.names=job1,job2
spring.batch.job.enabled=true
spring.batch.initializer.enabled=true
spring.batch.schema= # batch schema to load

# AOP
spring.aop.auto=
spring.aop.proxy-target-class=

# FILE ENCODING (FileEncodingApplicationListener)
spring.mandatory-file-encoding=false

# SPRING SOCIAL (SocialWebAutoConfiguration)
spring.social.auto-connection-views=true # Set to true for default connection views or false if you provide your own

# SPRING SOCIAL FACEBOOK (FacebookAutoConfiguration)
spring.social.facebook.app-id= # your application's Facebook App ID
spring.social.facebook.app-secret= # your application's Facebook App Secret

# SPRING SOCIAL LINKEDIN (LinkedInAutoConfiguration)
spring.social.linkedin.app-id= # your application's LinkedIn App ID
spring.social.linkedin.app-secret= # your application's LinkedIn App Secret

# SPRING SOCIAL TWITTER (TwitterAutoConfiguration)
spring.social.twitter.app-id= # your application's Twitter App ID
spring.social.twitter.app-secret= # your application's Twitter App Secret

# SPRING MOBILE SITE PREFERENCE (SitePreferenceAutoConfiguration)
spring.mobile.sitepreference.enabled=true # enabled by default

# SPRING MOBILE DEVICE VIEWS (DeviceDelegatingViewResolverAutoConfiguration)
spring.mobile.devicedelegatingviewresolver.enabled=true # disabled by default
spring.mobile.devicedelegatingviewresolver.normal-prefix=
spring.mobile.devicedelegatingviewresolver.normal-suffix=
spring.mobile.devicedelegatingviewresolver.mobile-prefix=mobile/
spring.mobile.devicedelegatingviewresolver.mobile-suffix=
spring.mobile.devicedelegatingviewresolver.tablet-prefix=tablet/
spring.mobile.devicedelegatingviewresolver.tablet-suffix=

# ----------------------------------------
# ACTUATOR PROPERTIES
# ----------------------------------------

# MANAGEMENT HTTP SERVER (ManagementServerProperties)
management.port= # defaults to 'server.port'
management.address= # bind to a specific NIC
management.context-path= # default to '/'
management.add-application-context-header= # default to true
management.security.enabled=true # enable security
management.security.role=ADMIN # role required to access the management endpoint
management.security.sessions=stateless # session creating policy to use (always, never, if_required, stateless)

# PID FILE (ApplicationPidFileWriter)
spring.pidfile= # Location of the PID file to write

# ENDPOINTS (AbstractEndpoint subclasses)
endpoints.autoconfig.id=autoconfig
endpoints.autoconfig.sensitive=true
endpoints.autoconfig.enabled=true
endpoints.beans.id=beans
endpoints.beans.sensitive=true
endpoints.beans.enabled=true
endpoints.configprops.id=configprops
endpoints.configprops.sensitive=true
endpoints.configprops.enabled=true
endpoints.configprops.keys-to-sanitize=password,secret,key # suffix or regex
endpoints.dump.id=dump
endpoints.dump.sensitive=true
endpoints.dump.enabled=true
endpoints.env.id=env
endpoints.env.sensitive=true
endpoints.env.enabled=true
endpoints.env.keys-to-sanitize=password,secret,key # suffix or regex
endpoints.health.id=health
endpoints.health.sensitive=true
endpoints.health.enabled=true
endpoints.health.mapping.*= # mapping of health statuses to HttpStatus codes
endpoints.health.time-to-live=1000
endpoints.info.id=info
endpoints.info.sensitive=false
endpoints.info.enabled=true
endpoints.mappings.enabled=true
endpoints.mappings.id=mappings
endpoints.mappings.sensitive=true
endpoints.metrics.id=metrics
endpoints.metrics.sensitive=true
endpoints.metrics.enabled=true
endpoints.shutdown.id=shutdown
endpoints.shutdown.sensitive=true
endpoints.shutdown.enabled=false
endpoints.trace.id=trace
endpoints.trace.sensitive=true
endpoints.trace.enabled=true

# HEALTH INDICATORS
management.health.db.enabled=true
management.health.diskspace.enabled=true
management.health.mongo.enabled=true
management.health.rabbit.enabled=true
management.health.redis.enabled=true
management.health.solr.enabled=true
management.health.diskspace.path=.
management.health.diskspace.threshold=10485760
management.health.status.order: DOWN, OUT_OF_SERVICE, UNKNOWN, UP

# MVC ONLY ENDPOINTS
endpoints.jolokia.path=jolokia
endpoints.jolokia.sensitive=true
endpoints.jolokia.enabled=true # when using Jolokia

# JMX ENDPOINT (EndpointMBeanExportProperties)
endpoints.jmx.enabled=true
endpoints.jmx.domain= # the JMX domain, defaults to 'org.springboot'
endpoints.jmx.unique-names=false
endpoints.jmx.static-names=

# JOLOKIA (JolokiaProperties)
jolokia.config.*= # See Jolokia manual

# REMOTE SHELL
shell.auth=simple # jaas, key, simple, spring
shell.command-refresh-interval=-1
shell.command-path-patterns= # classpath*:/commands/**, classpath*:/crash/commands/**
shell.config-path-patterns= # classpath*:/crash/*
shell.disabled-commands=jpa*,jdbc*,jndi* # comma-separated list of commands to disable
shell.disabled-plugins=false # don't expose plugins
shell.ssh.enabled= # ssh settings ...
shell.ssh.key-path=
shell.ssh.port=
shell.telnet.enabled= # telnet settings ...
shell.telnet.port=
shell.auth.jaas.domain= # authentication settings ...
shell.auth.key.path=
shell.auth.simple.user.name=
shell.auth.simple.user.password=
shell.auth.spring.roles=

# GIT INFO
spring.git.properties= # resource ref to generated git info properties file
```

## B. 메타데이터 설정<a name="B. 메타데이터 설정"></a>
스프링부트 jars는 설정 속성들을 모두 지원하는 메타데이터 파일과 함께 제공된다. 이 파일들은 IDE 개발자가 제공하는 문맥적인 도움과 사용자가 ```application.properties``` 혹은 ```application.yml``` 파일에서 처럼 "코드 완성"기능을 허용하도록 설계되었다.

메타데이터 파일의 대부분은 ```@ConfigurationProperties``` 선언된 모든 아이템을 컴파일하는 과정에서 자동적으로 생성된다.

### B.1. 메타데이터 형식<a name="B.1. 메타데이터 형식"></a>
설정 메타데이터 파일은 jar 안쪽에 ```META-INF/spring-configuration-metadata.json```에 위치한다. 간단한 JSON 형식에 아이템들은 "groups" 혹은 "properties" 하위에 분류되어 있다:

```
{"groups": [
    {
        "name": "server",
        "type": "org.springframework.boot.autoconfigure.web.ServerProperties",
        "sourceType": "org.springframework.boot.autoconfigure.web.ServerProperties"
    }
    ...
],"properties": [
    {
        "name": "server.port",
        "type": "java.lang.Integer",
        "sourceType": "org.springframework.boot.autoconfigure.web.ServerProperties"
    },
    {
        "name": "server.servlet-path",
        "type": "java.lang.String",
        "sourceType": "org.springframework.boot.autoconfigure.web.ServerProperties"
        "defaultValue": "/"
    }
    ...
]}
```

각 "property"는 사용자가 정의한 값으로 설정되어 있다. 예를 들어 ```server.port``` 그리고 ```server.servlet-path```는 ```application.properties``` 에 다음과 같이 정의되어 있다:

```
server.port=9090
server.servlet-path=/home
```

"groups"는 사용자정의되지 않은 높은 수준의 것들이지만 프로퍼티즈를 위한 문맥적인 그룹핑을 제공한다. 예를 들어 ```server.port``` 그리고 ```server.servlet-path``` 속성은 ```server``` 그룹의 일부분이다.

> 노트:
모든 "property"이 "group"을 필요로 하지는 않는다. 일부 프로퍼티즈들에 존재한다.

#### B.1.1. 그룹 어트리뷰트<a name="B.1.1. 그룹 어트리뷰트"></a>
```groups```로 구성된 JSON 객체배열은 다음 속성들을 따른다:

| 이름 | 유형 | 목적 |
|------|------|------|
|```name```|String|그룹의 완전한 경로, 이 속성은 필수항목이다. |
|```type```|String|그룹의 데이터 타입의 클래스명. 예를들어, 그룹이 ```@ConfigurationProperties``` 주석 클래스를 기반으로 한 경우 속성은 해당래스의 완전한 이름을 포함한다. |
|```description```|String|사용자에게 노출되는 그룹에 대한 짧은 설명. 설명이 없는 경우는 생략할 수 있다. 설명은 짧은 단락들로, 그 중에서 첫번째 줄에는 간결한 요약을 제공하는 것이 좋다.|
|```sourceType```|String|이 그룹에 관여하는 소스의 클래스 이름. 예를 들어 ```@ConfigurationProperties``` 으로 선언된 ```@Bean``` 메서드에 따라 이 속성은 메서드를 포함하는 ```@Configuration``` 클래스의 완전한 이름을 포함한다. |
|```sourceMethod```|String|이 그룹에 관여된 메서드의 완전한 이름(괄호와 인수 유형을 포함). 예를 들어, ```@ConfigurationProperties``` 선언된 ```@Bean``` 메서드의 이름. 소스 메서드가 알려지지 않은 경우 생략할 수 있다. |

#### B.1.2. 속성 어트리뷰트<a name="B.1.2. 속성 어트리뷰트"></a>
속성 배열에 포함된 JSON 객체는 다음과 같은 속성들을 포함할 수 있다:

| Name | Type | Purpose |
|------|------|---------|
|```name```|String|속성의 완전한 이름. 이름은 소문자-로 되어있다(예: ```server.servlet-path```). 이 속성은 필수항목이다. |
|```type```|String|속성의 데이터 유형의 클래스 이름. 예를 들어, ```java.lnag.String```. 이 특성은 입력할 수 있는 값의 종류로 사용자를 안내하는데 사용될 수 있다. 일관성을 위해, 원시종류는 래퍼 대응을 통해 지정된다, 예를 들어 ```boolean```은 ```java.lang.Boolean```이 된다. 컬렉션 유형은 그들의 인터페이스에 대응하고 실제 제네릭 타입들을 정의한다, 예를 들어 ``` java.util.HashMap<java.lang.String,java.lang.Integer>```는 ```java.util.Map<java.lang.String,java.lang.Integer>```가 된다. 보다 복잡한 타입의 클래스가 될 경우에는 값은 문자열로 변환되어 연결된다. |
|```description```|String|사용자에게 노출되는 그룹에 관한 짧은 설명. 설명이 없는 경우는 생략할 수 있다. 설명이 짧은 문단인 경우에는 간결한 요약을 첫번째 줄에 제공하는 것을 권장한다. 설명의 마지막 라인에는 마침표(.)으로 끝을 기술한다. |
|```sourceType```|String|이 속성은 소스의 클래스명을 제공한다. 예를 들어, ```@ConfigurationProperties``` 선언된 클래스의 속성은 클래스의 완전한 이름을 포함한다. 소스 유형이 알려지지 않은 경우에는 생략될 수 있다. |
|```defaultValue```|Object|속성이 지정되지 않았을 때 사용되는 기본값이다. 속성의 타입이 배열인 경우는 값의 배열일 수 있다. 소스 유형이 알려지지 않은 경우에는 생략될 수 있다. |
|```deprecated```|boolean|속성을 더이상 사용하지 않을 경우 정의한다. deprecated 필드를 정의하지 않았거나 정보가 알려지지 않은 경우 생략될 수 있다. |

#### B.1.3. 반복적인 메타데이터 아이템<a name="B.1.3. 반복적인 메타데이터 아이템"></a>
"property"와 "group" 객체에 대한 완벽한 허용은 메타-데이터 파일 내에서 같은 이름이 여러번 반복될 수 있다. 예를 들어, 스프링부트는 Hikari, Tomcat 그리고 DBCP 클래스들에 대한  ```spring.datasource``` 속성들의 이름들에 대한 잠재적인 중복을 제공한다. 메타-데이터의 소비는 시나리오들을 지원할수 있도록 주의를 기울여야 한다.

### B.2. 애노테이션 프로레서를 사용하여 메타데이터 생성<a name="B.2. 애노테이션 프로레서를 사용하여 메타데이터 생성"></a>
```spring-boot-configuration-processor``` jar 를 사용하여 ```@ConfigurationProperties``` 선언된 아이템들로부터 설정 메타-데이터 파일을 쉽게 생성할 수 있다. jar에 포함된 Java annotation processor는 프로젝트를 컴파일할 때 요청한다. 프로세서를 사용하려면, ```spring-boot-configuration-processor```을 선택적으로 의존성을 포함, 메이븐의 경우는 다음과 같이 추가할 수 있다:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-configuration-processor</artifactId>
    <optional>true</optional>
</dependency>
```

애노테이션은 ```@ConfigurationProperties```을 사용한 클래스와 메서드들을 추출한다. 설정클래스들의 필드값들은 Javadoc의 ```description``` 속성으로 사용된다.

> 노트:
JSON에 추가되기 전에 처리되지 않기 때문에 ```@ConfigurationProperties``` 필드 Javadoc과 간단한 텍스트를 사용한다.

#### B.2.1. 내부 속성<a name="B.2.1. 내부 속성"></a>
애노테이션 프로세서는 자동으로 중첩된 속성으로 내부 클래스를 고려할 것이다. 예를 들어, 다음 클래스의 경우:

```java
@ConfigurationProperties(prefix="server")
public class ServerProperties {

    private String name;

    private Host host;

    // ... getter and setters

    private static class Host {

        private String ip;

        private int port;

        // ... getter and setters

    }

}
```

는 ```server.name```, ```server.host.ip``` 과 ```server.host.port``` 속성들을 생성한다. 중첩된 것처럼 일반(내부 클래스가 아닌) 클래스가 처리되어야한다는 것을 나타내기 위해서 ```@NestedConfigurationProperty``` 애노테이션을 사용할 수 있다.

#### B.2.2. 추가적인 메타데이터 추가<a name="B.2.2. 추가적인 메타데이터 추가"></a>
스프링부트의 설정파일 제어는 매우 유연하며, 프로퍼타이즈가 ```@ConfigurationProperties``` 빈에 연결되지 않는 경우가 종종 존재한다. 각각의 경우, 애노테이션 프로세스가 자동으로 주요 메타-데이터 파일에 ```META-INF/additional-spring-configuration-metadata.json```의 아이템들을 병합한다.

```additional-spring-configuration-metadata.json``` 파일의 형식은 ```spring-configuration-metadata.json``` 파일과 같다. 추가 프로퍼타이즈 파일은 선택적이며, 추가 프로퍼타이즈가 없다면, 추가하지 않는다.

## C. 자동설정 클래스<a name="자동설정 클래스"></a>
스프링부트에서 제공하는 자동설정 클래스들의 문서와 소스코드 링크를 제공하는 목록이 여기 있다. 애플리케이션의 자동설정 보고서에 관한 보다 자세한 기능들을 볼 수 있도록 켤 수 있는 것이 가능하다(앱을 시작할 때 ```--debug``` 혹은 ```-Ddebug```, 혹은 애플리케이션의 액츄에이터 중 ```autoconfig``` 엔드포인트를 사용한다).

### C.1. "spring-boot-autoconfigure" 모듈<name="C.1. \"spring-boot-autoconfigure\" 모듈"></a>

```spring-boot-autoconfigure``` 모듈에 있는 자동설정 클래스들은 다음과 같다:
| 설정 클래스 | 링크 |
|[ActiveMQAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jms/activemq/ActiveMQAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/jms/activemq/ActiveMQAutoConfiguration.html) |
| [AopAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/aop/AopAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/aop/AopAutoConfiguration.html) |
| [BatchAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/batch/BatchAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/batch/BatchAutoConfiguration.html) |
| [CloudAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/cloud/CloudAutoConfiguration.java) | [http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/cloud/CloudAutoConfiguration.html](javadoc) |
| [DataSourceAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jdbc/DataSourceAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/jdbc/DataSourceAutoConfiguration.html) |
| [DataSourceTransactionManagerAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/jdbc/DataSourceTransactionManagerAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/jdbc/DataSourceTransactionManagerAutoConfiguration.html) |
| [DeviceDelegatingViewResolverAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/mobile/DeviceDelegatingViewResolverAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/mobile/DeviceDelegatingViewResolverAutoConfiguration.html) |
| [DeviceResolverAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/mobile/DeviceResolverAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/mobile/DeviceResolverAutoConfiguration.html) |
| [DispatcherServletAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/web/DispatcherServletAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/web/DispatcherServletAutoConfiguration.html) |
| [ElasticsearchAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/elasticsearch/ElasticsearchAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/elasticsearch/ElasticsearchAutoConfiguration.html) |
| [ElasticsearchDataAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/elasticsearch/ElasticsearchDataAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/elasticsearch/ElasticsearchDataAutoConfiguration.html) |
| [EmbeddedServletContainerAutoConfiguration](http://github.com/spring-projects/spring-boot/tree/master/spring-boot-autoconfigure/src/main/java/org/springframework/boot/autoconfigure/web/EmbeddedServletContainerAutoConfiguration.java) | [javadoc](http://docs.spring.io/spring-boot/docs/1.2.0.BUILD-SNAPSHOT/api/org/springframework/boot/autoconfigure/web/EmbeddedServletContainerAutoConfiguration.html) |


### C.2. "spring-boot-actuator" 모듈<a name="C.2. \"spring-boot-actuator\" 모듈"></a>

## D. 실행가능한 jar 형식<a name="D. 실행가능한 jar 형식"></a>
```spring-boot-loader``` 모듈은 스프링부트가 실행가능한 jar와 war 파일을 지원하도록 허용한다. 만약 메이븐과 그레들 플러그인을 사용한다면, 실행가능한 jar는 자동적으로 생성되며 어떤 식으로 작업이 진행되는지를 세부적으로 알 필요는 없다.

만약 다른 빌드 시스템을 통해서 실행가능한 jar를 생성해야한다면, 혹은 기저에 깔린 기술들에 대해서 강한 호기심이 있다면, 이 섹션은 배경지식을 제공해줄 것이다.

### D.1. 내부 JARs
자바는 기본적으로 jar 파일들을 내장하는 어떤 방식도 제공하지 않는다(예를 들어 jar 파일은 jar 파일 내에 자신들을 포함한다). 이것은 압축해제 없이 커맨드라인에서 자급자족하는 애플리케이션 배포시에는 문제가 될 수 있다.

그 해결책으로, 많은 개발자들은 'shaded' jar를 사용한다. 'shaded' jar는 'uber jar' 라는 간단한 형태에 모든 jar, 모든 클래스를 간단하게 묶는다. shaded jar의 문제점은 애플리케이션에서 실제로 사용할 때 라이브러리들을 찾기가 힘들다는 것이다. 이는 또한 다양한 jar 안에 같은 파일명을 사용하는 경우 문제(하지만 내용은 다른)가 될 수 있다. 스프링부트는 실제 내부 jar에 접근하는 방식을 다르게 접근하였다.

#### D.1.1. 실행가능한 jar 파일 구조<a name="D.1.1. 실행가능한 jar 파일 구조"></a>
스프링부트 로더는 양립하는 jar 파일들을 다음과 같은 방법으로 구성한다.

```
example.jar
 |
 +-META-INF
 |  +-MANIFEST.MF
 +-org
 |  +-springframework
 |     +-boot
 |        +-loader
 |           +-<spring boot loader classes>
 +-com
 |  +-mycompany
 |     + project
 |        +-YouClasses.class
 +-lib
    +-dependency1.jar
    +-dependency2.jar
```

의존성 라이브러리들은 내부에 ```lib``` 디렉토리에 위치시킨다.

#### D.1.2. 실행가능한 war 파일 구조<a name="D.1.2. 실행가능한 war 파일 구조"></a>
스프링부트 로더는 양립하는 war 파일을 다음과 같은 방법으로 구성한다.

```
example.jar
 |
 +-META-INF
 |  +-MANIFEST.MF
 +-org
 |  +-springframework
 |     +-boot
 |        +-loader
 |           +-<spring boot loader classes>
 +-WEB-INF
    +-classes
    |  +-com
    |     +-mycompany
    |        +-project
    |           +-YouClasses.class
    +-lib
    |  +-dependency1.jar
    |  +-dependency2.jar
    +-lib-provided
       +-servlet-api.jar
       +-dependency3.jar
```

의존성 라이브러리들은 ```WEB-INF/lib``` 디렉토리에 위치시킨다. 실행하는데는 필요하지만 전통적인 웹 컨테이너에 배포하는 경우에는 필요하지 않은 의존성 라이브러리들은 ```WEB-INF/lib-provided```에 위치시킨다.

### D.2.  스프링부트의 "JarFile" 클래스<a name="D.2. 스프링부트의 \"JarFile\" 클래스"></a>
내장된 jar를 지원하는 핵심 클래스는 ```org.springframework.boot.loader.jar.JarFile```를 사용한다. 이 클래스는 표준 jar 파일로부터 혹은 내부 하위에 있는 jar data로부터 jar 내용을 읽어오는 것을 허용한다. 처음 적재될 때, 각각의 ```JarEntry```의 위치는 외부 jar의 물리적 파일에 상쇄되어 배치된다.

```
myapp.jar
+---------+---------------------+
|         | /lib/mylib.jar      |
| A.class |+---------+---------+|
|         || B.class | B.class ||
|         |+---------+---------+|
+---------+---------------------+
^          ^          ^
0063       3452       3980
```

위의 예를 살펴보면 ```myapp.jar``` 내에서 ```0063```에 위치한 ```A.class```를 어떻게 찾는 지 볼 수 있다. ```myapp.jar``` 내에서 ```B.class``는 ```3452```와 ```3980```위치해있다.

여기서 알 수 있는건, 외부의 jar에 접근하는 방식으로 내부의 엔트리들을 쉽게 읽어올 수 있다. 우리는 압축을 해제할 필요가 없고 모든 엔트리 데이터를 메모리에서 읽어올 필요도 없다.

#### D.2.1. 표준 자바 "JarFile" 의 호환성<a name="D.2.1. 표준 자바 \"JarFile\" 의 호환성"></a>
스프링부트 로더는 존재하는 코드와 라이브러리들이 양립할수 있도록 노력한다. ```java.util.jar.JarFile```에서 확장한 ```org.springframework.boot.loader.jar.JarFile```은 잘못된 부분들을 교환한다. ```RandomAccessJarFile.getURL()``` 메서드는 ```java.net.JarURLConnection``` 양립가능한 커넥션 ```URL```을 반환할 것이다. ```RandomAccessJarFile``` URL은 Java의 ```URLClassLoader```로 사용가능하다.

### D.3. 실행가능한 jars 실행<a name="D.3. 실행가능한 jars 실행"></a>
```org.springframework.boot.loader.Launcher``` 클래스는 실행가능한 jar의 주진지점(main entry point)로 사용되는 부트스트랩 클래스다. jar 파일에 ```Main-Class``` 이며 ```URLClassLoader```에 접근하여 최종적으로 ```method()``` 메서드를 호출하도록 설정된다.

하위클래스 3 런처(```JarLauncher```, ```WarLauncher``` 그리고 ```PropertiesLauncher```)가 있다. 이 클래스들의 용도는 내부 jar 파일 혹은 war 파일의 디렉토리에서 자원(```.class``` 파일 등)을 읽는 것이다(클래스패스에 따라 제공한다). ```[Jar|War]Launcher```의 경우 내장 경로는 고정적(war의 경우 ```lib/*.jar``` 그리고  ```lib-provided/*.jar```)이다 추가적으로 jar를 저 위치에 추가하면 된다.
```PropertiesLauncher```는 기본적으로 ```lib/``` 를 살펴보지만,  ```application.properties``` 에서 ```LOADER_PATH``` 혹은 ```loader.path``` 환경변수로 설정한 위치에 추가할수 있다(콤마로 디렉토리나 압축파일의 위치를 지정한다).

#### D.3.1. 매니페스트 실행<a name="D.3.1. 매니페스트 실행"></a>
```Launcher```가 실행하려면 ```META-INF/MANIFEST.MF``` 의 ``Main-Class``` 속성을 정의해야 한다. 실제로 실행하기를 바라는 클래스는 ```Start-Class``` 속성으로 정의하고 싶을 것이다(예, ```method``` 메서드를 작성한 클래스).

예를 들어, 여기 실행 jar 파일에 있는 전통적인 ```MANIFEST.MF```가 있다.

```
Main-Class: org.springframework.boot.loader.JarLauncher
Start-Class: com.mycompany.project.MyApplication
```

다음은 war 파일의 경우:

```
Main-Class: org.springframework.boot.loader.WarLauncher
Start-Class: com.mycompany.project.MyApplication
```

> 노트
매니페스트 파일에 ```Class-Path``` 엔트리를 정의할 필요는 없다. 내장 jar 파일로 부터 추출한다.

#### D.3.2. 아카이브 확장<a nam="D.3.2. 아카이브 확장"></a>
PaaS 구현체들은 실행에 앞서 압축파일을 압축해제하는 선택을 할 것이다. 예를 들어, Cloud Foundry 는 이 방법을 수행한다. 런처가 실행될 때 간단하게 압축해제하도록 할 수 있다:

```
$ unzip -q myapp.jar
$ java org.springframework.boot.loader.JarLauncher
```

### D.4. ```PropertiesLauncher``` 기능들<a name="D.4. PropertiesLauncher 기능들"></a>
```PropertiesLauncher```는 확장 프로퍼티즈를 활성화할 수 있는 특별한 기능을 가진다(System properties, environment variables, manifest entries or application.properties).

| KEY | Purpose |
|-----|---------|
|```loader.path```| 콤마(,)로 구분된 클래스패스(예, ```lib:${HOME}/app/lib```)
> 역자주: 그런데 왜 예에는 콜론...이지? |
| ```loader.home``` | 추가적인 프로퍼티즈 파일 위치 예: ```/opt/app``` (기본 ```${user.dir}```) |
| ```loader.args``` | (스페이스로 구분된) 메인메서드의 인자 |
| ```loader.main``` | 실행 기본 클래스명, 예: ```com.app.Application``` |
| ```loader.config.name``` | 프로퍼티즈 파일명, 예: ```loader``` (기본적으로 ```application```) |
| ```loader.config.location``` | 프로퍼티즈 파일 경로, 예: ```classpath:loader.properties``` (기본 ```application.properties```) |
| ```loader.system``` | 모든 프로퍼티즈를 시스템 프로퍼티즈에 추가할 것인지를 정의(기본 false) |

매니페스트 엔트리 키는 단어의 첫 글자를 대문자로 형성되고 "." 에서 "-"로 분리하여 변환한다(예: ```Loader-Path```). 예외는 ```JarLauncher```과의 호환성을 위해 매니페스트에 시작-클래스로 조회되는 ```loader.main```가 된다.

환경변수는 기간 대신 밑줄구분으로 대문자화한다.
* ```loader.home```은 ```loader.config.location```을 정의하지 않는 한 프로퍼티즈 파일의 디렉토리 경로다(기본을 오버라이딩).
* ```loader.path``` 디렉토리(jar 와 zip 파일들을 회귀적으로 살펴보는), 압축파일 경로 혹은 와일드카드 패턴(JVM의 기본적인 행동)를 포함할 수 있다.
* placeholder 는 시스템과 환경변수를 더해 사용전 프로퍼티즈 파일의 모든 값을 대체한다.

### D.5. 실행가능한 jar 제약사항
몇몇 제약사항들 대문에 스프링부트 로더로 압축된 애플리케이션이 동작할 때 고려해야할 사항들이 있다.

#### D.5.1. Zip 엔트리 압축
내장된 jar ```ZipEntry```는 ```ZipEntry.STORED``` 메서드를 사용해서 저장해야 한다. 내장된 jar의 컨텐츠를 개별적으로 직접탐색할 수 있기 때문이다. 내장된 jar 파일의 컨텐츠는 외부 jar 안에 다른 항목들처럼 압축할 수 있다.

#### D.5.2. System ClassLoader
실행된 애플리케이션은 클래스를 로딩할 때(대부분의 라이브러리와 프레임웤가 기본적으로는 이렇게 한다) ```Thread.getContextClassLoader()```를 사용할 것이다. 내장된 jar의 클래스를 ```ClassLoader.getSystemClassLoader()```로 읽으려고 시도하면 실패할 것이다. ```java.util.Logging``` 를 사용하는 것은 항상 주의해야한다. 이런 이유로 다른 로깅 구현체를 고려해야 한다.

### D.6. 단독 jar 솔루션 대안
위의 제약사항으로 스프링부트로더를 사용할수 없다면 다음의 대안들을 고려해볼 수 있다:
* [Maven Shade Plugin](http://maven.apache.org/plugins/maven-shade-plugin/)
* [JarClassLoader](http://www.jdotsoft.com/JarClassLoader.php)
* [OneJar](http://one-jar.sourceforge.net/)

## E. 의존성 버전<a name="E. 의존성 버전"></a>UndertowBuilderCustomizer
