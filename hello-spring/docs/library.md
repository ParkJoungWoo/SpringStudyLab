# 라이브러리 공부
1. Gradle -> 빌드 관리자

Gradle, Maven --> 라이브러리의 의존을 관리해준다.

스프링에는 많은 라이브러리가 존재한다.
어떤 라이브러리 A가 B라는 라이브러리의 의존성이 있다면 빌드 관리자가 자동으로 가져온다.

과거 WAS에서 JAVA코드를 작성하는 방식(웹서버와 개발이 별개의 라이브러리였다.)
-> 요즘에는 라이브러리가 Embeded로 웹 서버가 내장되어있다.

출력은 System.out.println이 아닌 Log를 활용해서 출력한다.

spring-boot-starter-web
- spring-boot-starter-tomcat 톰캣(웹서버)
- spring-webmvc(스프링 웹 MVC)

spring-boot-starter-thymeleaf : 타임리프 템플릿 엔진(View)\
spring-boot-starter(공통) : 스프링 부트 + 스프링 코어 + 로깅
- spring-boot
    - spring-core
- spring-boot-starter-logging
  - logback, ⭐slf4j

테스트 라이브러리
- spring-boog-starter-test
  - junit : ⭐테스트 프레임워크
  - mockito : 목 라이브러리
  - assertj : 테스트 코드
  - spring-test : 스프링 통합 테스트 지원