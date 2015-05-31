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

# III. 스프링부트 사용
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
## 23. 외부설정
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
### 25.5. 로그 설정 변경
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
## 35. 테스팅
### 35.1. 테스트 스코프 의존성
### 35.2. 스프링 애플리케이션 테스트
### 35.3. 스프링부트 애플리케이션 테스트
#### 35.3.1. 스팍Spock을 사용하여 스프링 부트 애플리케이션 테스트
### 35.4. 테스트 유틸리티
#### 35.4.1. ```ConfigFileApplicationContextInitializer```
#### 35.4.2. ```EnvironmentTestUtils```
#### 35.4.3. ```OutputCapture```
#### 35.4.4. ```TestRestTemplate```
## 36. 자동설정으로 개발하고 @Condition 사용하기
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
## 40. 엔드포인트
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

# VII. 스프링부트 CLI
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
### 60.8. 변경된 그레들 설정으로 리패키징
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
### 64.7. 외부 속성들의 빌트인 항목 살펴보기
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
## 69. 데이터베이스 초기화
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

# I. 스프링부트 문서
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
* 빌드툴 플러그인: [메이븐](#스프링부트 메이븐 플러그인) | [그레들](#스프링부트 그레들 플러그인)
* 부록: [애플리케이션 속성](#애플리케이션 속성) | [자동설정 클래스](#자동설정 클래스) | [실행가능한 jar 형식](#실행가능한 jar 형식)

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

스프링부트 의존성은 ```org.springframework.boot group```을 사용하여 정의된다. 일반적으로 여러분의 프로젝트는 하나 혹은 그 이상 [스프링부트 스타터 POMs](#스프링부트 스타터 POMs)에 관한 의존성을 정의했을 것이다. 스프링부트는 의존성을 간단하게 정의하고 실행가능한 jars를 생성하는데 매우 유용한 [그레들 플러그인]($스프링부트 그레들 플러그인)을 제공한다.

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

### 10.2. 스프링부트 CLI를 이용한 설치
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

## 11. 초기 스프링부터 애플리케이션 개발<a name="초기 스프링부터 애플리케이션 개발"></a>
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

스프링부트는 이를 [다르게 접근](#실행가능한 jar 형식)하였고 실제로 내재하고 있는 jar파일들을 직접 접근가능하다.

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

## 13. 빌드 시스템
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

또한 [spring-boot-gradle-plugin](#스프링부트 그레들 플러그인)은 실행가능한 jar를 생성하는 태스크들을 제공하고 소스를 바탕으로 프로젝트를 실행하는 것이 가능하다. 거기다가 ```ResolutionStrategy```을 추가하여 [의존성의 버전넘버를 생략하는 것](#버전 없이 의존성 정의)도 가능하다:
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

### 22.4. 애플리케이션 이벤트와 리스너
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

## 23. 외부설정<a name="외부설정"></a>
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

### 23.5. Properties 대신 YAML 사용<a name="Properties 대신 YAML 사용"></a>
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

## 24. 프로파일<a name="프로파일"></a>
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

### 25.5. 로그 설정 변경

다양한 로깅 시스템은 기본적인 라이브러리를 포함하여 클래스패스 상의 활동상태를 관찰할 수 있다, 또한 클래스패스 루트에 위치한 적절한 설정파일을 제공하면 변경할 수 있으나, 스프링 ```Environment``` ```logging.config``` 속성으로 정의해야한다. (보충하자면, 로깅 시작은 ```ApplicationContext```가 **생성되기 전** 초기화되는 순간부터 시작된다. 스프링 ```@Configuration``` 파일에서 ```@PropertySources``` 에서 로깅을 컨트롤하는 것은 불가능하다. 시스템 프로퍼티즈와 스프링부트의 외부설정 파일을 이용한 것은 잘 동작한다. )

로깅시스템의 부수적인, 다음의 파일들이 있어야 한다:
| 로깅 시스템 | 설정파일 |
|------------|----------|
| Logback | logback.xml |
| Log4j | log4j.properties 혹은 log4j.xml |
| JDK(Java Util Logging) | logging.properties |

설정에 필요한 몇몇 속성들은 스프링 ```Envirionment``에서 시스템 프로퍼티스로 변환된다.
| Spring environment | System property | 설명 |
|--------------------|-----------------|------|
| logging.file | LOG_FILE | 정의되어 있다면 기본 로그 설정으로 사용된다. |
| lggging.path | LOG_PATH | 정의도어 있다면 기본 로그 설정으로 사용된다. |
| PID | PID | 현재 프로세스 ID(가능하다면 발견한 프로세스 ID를 사용하며 정의되어 있지 않은 경우에는 OS 환경 변수를 사용한다.) **재확인** |

모든 로깅 시스템에 대한 지원은 로깅 시스템의 설정 파일을 분석하여 시스템 프로퍼티스로 변환할 수 있기 때문이다. 예제로 ```spring-boot.jar``` 안에 기본 설정을 살펴보라.
> 위험: 실행가능한 JAR로 실행했을 때 Java Util Logging을 사용할 때 클래스로딩classloading 에서 문제가 발생한다는 이슈가 있다. 우리는 가능하면 이것을 피하기를 권장한다.

## 26. 웹 애플리케이션 개발
### 26.1. 'Spring Web MVC framework'<a name="Spring Web MVC framework"></a>
#### 26.1.1. Spring MVC 자동설정
#### 26.1.2. ```HttpMessageConverter```
#### 26.1.3. ```MessageCodesResolver```
#### 26.1.4. ```Static Content````
#### 26.1.5. Template engines
#### 26.1.6. 오류 제어, 웹스피어
#### 애플리케이션 서버에서 오류 제어
### 26.2. JAX-RS 그리고 Jersey
### 26.3. 내장형 서블릿 컨테이너 지원<a name="내장형 서블릿 컨테이너 지원"></a>
#### 26.3.1. 서블릿 그리고 필터
#### 26.3.2. ```EmbeddedWebApplicationContext```
#### 26.3.3. 내장형 서블릿 컨테이너 변경
#### 변경 작성방법
#### ```ConfigurableEmbeddedServletContainer``` 직접 변경
#### 26.3.4. JSP 제약사항
## 27. 보안
## 28. SQL 데이터베이스 작업<a name="SQL 데이터베이스 작업"></a>
### 28.1. 데이터베이스 설정
#### 28.1.1. 내장형 데이터베이스 지원
#### 28.1.2. 외부 데이터베이스 연결
#### 28.1.3. JNDI 데이터베이스 연결
### 28.2. JdbcTemplate 사용
### 28.3. JPA 그리고 'Spring Data'
#### 28.3.1. 엔티티 클래스
#### 28.3.2. Spring Data JPA 레파지토리
#### 28.3.3. JPA 데이터베이스 생성 및 삭제
## 29. NoSQL 기술 작업<a name="NoSQL 기술 작업"></a>
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
## 30. 메시징<a name="메시징"></a>
### 30.1. JMS<a name="JMS"></a>
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
## 35. 테스팅<a name="테스팅"></a>
### 35.1. 테스트 스코프 의존성
### 35.2. 스프링 애플리케이션 테스트
### 35.3. 스프링부트 애플리케이션 테스트<a name="스프링부트 애플리케이션 테스트"></a>
#### 35.3.1. 스팍Spock을 사용하여 스프링 부트 애플리케이션 테스트
### 35.4. 테스트 유틸리티<a name="테스트 유틸리티"></a>
#### 35.4.1. ```ConfigFileApplicationContextInitializer```
#### 35.4.2. ```EnvironmentTestUtils```
#### 35.4.3. ```OutputCapture```
#### 35.4.4. ```TestRestTemplate```
## 36. 자동설정으로 개발하고 @Condition 사용하기<a name="자동설정으로 개발와 상황에 맞춰 사용"></a>
### 36.1. 자동설정 빈 이해
### 36.2. 자동설정 위치 후보지
### 36.3. 컨디션 애노테이션 @Condition<a name="컨디션 애노테이션 @Condition"></a>
#### 36.3.1. 클래스 상황
#### 36.3.2. 빈Bean 상황
#### 36.3.3. 리소스 상황
#### 36.3.4. 웹 애플리케이션 상황
#### 36.3.5. SpEL 표현식 상황
## 37. 웹소켓
## 38. 다음 읽을거리

# V. 스프링부트 액츄에터: 출시준비 기능들<a name="스프링부트 액츄에터: 출시준비 기능들"></a>
## 39. 사용가능한 출시준비 기능들
## 40. 엔드포인트<a name="엔드포인트"></a>
### 40.1. 엔드포인트 변경<a name="엔드포인트 변경"></a>
### 40.2. 상태 정보 변경
### 40.3. 애플리케이션 정보 안내 변경
#### 40.3.1. 빌드 시간에 관한 속성 확장 자동화
#### 메이븐을 이용하여 속성 확장 자동화
#### 그레들을 이용하여 속성 확장 자동화
#### 40.3.2. 깃 커밋 정보
## 41. HTTP를 통해서 모니터링 및 관리<a name="HTTP를 통해서 모니터링 및 관리"></a>
### 41.1. 세밀한 엔드포인트 노출
### 41.2. 관리 서버컨텍스트패스 변경
### 41.3. 관리 서버포트 변경
### 41.4. 관리 서버주소 변경
### 41.5. HTTP 엔드포인트 비활성화
### 41.6. 상태 엔드포인트에 대한 무기명 접근 제한
## 42. JMX를 통한 모니터링 및 관리<a name="JMX를 통한 모니터링 및 관리"></a>
### 42.1. MBean 이름 변경
### 42.2. JMX 엔드포인트 비활성화.
### 42.3. JMX용 Jolokia를 HTTP를 통해서 사용
#### 42.3.1. Jolokia 변경
#### 42.3.1. Jolokia 비활성화
## 43. 리모트쉘을 사용하여 모니터링 및 관리<a name="리모트쉘을 사용하여 모니터링 및 관리"></a>
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
## 45. 감시auditing<a name="감시auditing"></a>
## 46. 추적Tracing<a name="추적Tracing"></a>
### 46.1. 추적 변경
## 47. 프로세스 모니터링
### 47.1. 설정 확장
### 47.2. 작성
## 48. 다음 읽을거리

# VI. 클라우드 배포
## 49. Cloud Foundry<a name="Cloud Foundry"></a>
### 49.1. 서비스 연결
## 50. Heroku<a name="Heroku"></a>
## 51. CloudBees<a name="CloudBees"></a>
## 52. Openshift
## 53. Google App Engine
## 54. 다음 읽을거리

# VII. 스프링부트 CLI<a name="스프링부트 CLI"></a>
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
## 59. 스프링부트 메이븐 플러그인<a name="스프링부트 메이븐 플러그인"></a>
### 59.1. 플러그인 추가
### 59.2. 실행가능한 jar 와 war 파일 패키징
## 60. 스프링부트 그레들 플러그인<a name="스프링부트 그레들 플러그인"></a>
### 60.1. 플러그인 추가
### 60.2. 버전 없이 의존성 정의<a name="버전 없이 의존성 정의"></a>
#### 60.2.1. 버전 관리 변경
### 60.3. 기본적인 배제 원칙
### 60.4. 실행가능한 jar 와 war 파일 패키징
### 60.5. 프로젝트 바로 실행
### 60.6. 스프링부트 플러그인 설정
### 60.7. 리패키징 설정
### 60.8. 변경된 그레들 설정으로 리패키징
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

# IX. '어떻게How-to' 가이드<a name="'어떻게How-to' 가이드"></a>
혹시 우리가 대비하지 못한 부분들에서 문제들이 발생한다면 [스택오버플로우](http://stackoverflow.com/tags/spring-boot)에서 이미 누군가가 작성한 답변을 확인할 수도 있다: 이곳은 새로운 질문을 올리기에도 좋은 곳이다(```spring-boot``` 태그를 사용하자).

# 63. 스프링부트 애플리케이션
### 63.1. 자동설정 문제해결
### 63.2. 시작 전 ```Environment``` 혹은 ```ApplicationContext``` 변경
### 63.3. ```ApplicationContext``` 계층 빌드(부모 혹은 루트 컨텍스트 추가)
### 63.4. non-web 애플리케이션 생성
## 64. 속성 및 설정
### 64.1. 스프링애플리케이션의 설정 확장
### 64.2. 애플리케이션의 외부 속성 위치 변경
### 64.3. '간략한' 커맨드라인 인자 사용<a name="'간략한' 커맨드라인 인자 사용"></a>
### 64.4. 외부 속성을 YAML로 정의
### 64.5. 활성 스프링 프로파일 설정
### 64.6. <a href="환경 의존적 설정 변경">환경 의존적 설정 변경</a>
### 64.7. 외부 속성들의 빌트인 항목 살펴보기
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
## 69. 데이터베이스 초기화
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
### 74.8. 앤트를 이용해서 실행가능한 아카이브 빌드<a name="앤트를 이용해서 실행가능한 아카이브 빌드"></a>
## 75. 전통적 배포
### 75.1. 배포가능한 war 파일 생성
### 75.2. 오래된 서블릿 컨테이너에 배포가능한 war 파일 생성
### 75.3. 기존의 애플리케이션을 스프링부트로 변환
### 75.4. 웹로직을 위한 war 배포
### 75.5. 오래된(Servlet 2.5) 컨테이너에 war 배포

# X. 부록
## A. 일반적인 애플리케이션 속성<a name="애플리케이션 속성"></a>
## B. 메타데이터 설정
### B.1. 메타데이터 형식
#### B.1.1. 그룹 어트리뷰트
#### B.1.2. 속성 어트리뷰트
#### B.1.3. 반복적인 메타데이터 아이템
### B.2. 애노테이션 프로레서를 사용하여 메타데이터 생성
#### B.2.1. 내부 속성
#### B.2.2. 추가적인 메타데이터 추가
## C. 자동설정 클래스<a name="자동설정 클래스"></a>
### C.1. "spring-boot-autoconfigure" 모듈
### C.2. "spring-boot-actuator" 모듈
## D. 실행가능한 jar 형식<a name="실행가능한 jar 형식"></a>
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
