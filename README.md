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
## 14. 코드 구조
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
* 좋은 연습거리: [코드 구조](#코드 구조) | [@Configuration](#설정@Congiruation 클래스들) | [@EnableAutoConfiguration](#자동설정(Auto-configuration)) | [Beans and Dependency Inject](#스프링 빈과 의존성 주입)
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
|```spring-boot-starter-thymeleaf``|Support for the Thymeleaf templating engine, including integration with Spring.|
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


## 14. 코드 구조<a name="코드 구조"></a>
### 14.1. 'default' 패키지 이용
### 14.2. 메인 애플리케이션 클래스 위치
## 15. 설정@Congiruation 클래스들<a name="설정@Congiruation 클래스들"></a>
### 15.1. 추가된 설정 클래스들 불러오기
### 15.2. XML 설정 불러오기
## 16. 자동설정(Auto-configuration)<a name="자동설정(Auto-configuration)"></a>
### 16.1. 점진적으로 자동설정을 대체
### 16.2. 특정한 자동설정을 비활성화
## 17. 스프링 빈과 의존성 주입<a name="스프링 빈과 의존성 주입"></a>
## 18. ```@SpringBootApplication```애노테이션 사용
## 19. 애플리케이션 실행
### 19.1. IDE에서 실행<a name="IDE에서 실행"></a>
### 19.2. 패키징된 애플리케이션 실행<a name="패키징된 애플리케이션 실행"></a>
### 19.3. 메이븐 플러그인 이용<a name="메이븐 플러그인 이용"></a>
### 19.4. 그레들 플러그인 이용<a name="그레들 플러그인 이용"></a>
### 19.5. 핫스와핑
## 20. 출시를 위한 애플리케이션 패키징<a name="출시를 위한 애플리케이션 패키징"></a>
## 21. 다음 읽을거리

# IV. 스프링부트 기능<a name="스프링부트 기능"></a>
## 22. 스프링애플리케이션<a name="스프링애플리케이션"></a>
### 22.1. 배너 수정
### 22.2. 스프링애플리케이션 수정
### 22.3. 플루언트 빌더 API
### 22.4. 애플리케이션 이벤트와 리스너
### 22.5. 웹 환경
### 22.6. 커맨드라인러너 사용
### 22.7. 애플리케이션 종료
## 23. 외부설정<a name="외부설정"></a>
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
## 24. 프로파일<a name="프로파일"></a>
### 24.1. 활성프로파일 추가
### 24.2. 프로파일 작성방법
### 24.3. 프로파일 상세 설정파일
## 25. 로깅<a name="로깅"></a>
### 25.1. 로그 형식
### 25.2. 콘솔 출력
### 25.3. 파일 출력
### 25.4. 로그 레벨
### 25.5. 로그 설정 변경
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
