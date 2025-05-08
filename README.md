# 새모임 프로젝트🕊️
> 오프라인에서 취미활동을 함께 하거나, 혼자서는 갈 수 없는 곳에 함께 갈 파티원을 모집할 수 있는 서비스

<img src="src/main/documents/saemoim.png">

___ 
### 프로젝트 설명 </br>
새로운(New) 모임, 새(Bird)처럼 자유로운 모임 <br>
무엇이든지 함께 할 사람들을 구할 수 있는 새모임 프로젝트. <br>
오프라인 파티원 모집 플랫폼으로 모임을 생성하고 참여할 수 있으며, <br>
각 모임의 참여자들은 게시판을 이용해 모임 구성원들과 소통할 수 있습니다.
___
### 기술 스택</br>
[![My Skills](https://skillicons.dev/icons?i=java,spring,gradle,hibernate)](https://skillicons.dev) <br>

[![My Skills](https://skillicons.dev/icons?i=html,css,js,jquery)](https://skillicons.dev)

[![My Skills](https://skillicons.dev/icons?i=idea,git,github)](https://skillicons.dev)

[![My Skills](https://skillicons.dev/icons?i=mysql,redis)](https://skillicons.dev) <br>

<div>
  <img src="https://img.shields.io/badge/spring boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=Spring-Security&logoColor=white"> <br>
  <img src="https://img.shields.io/badge/JSON_Web_Token-EF2D5E?style=for-the-badge&logo=JSON Web Tokens&logoColor=000000"> <br>
  <img src="https://img.shields.io/badge/Amazon Ec2-232f3e?style=for-the-badge&logo=Amazon EC2&logoColor=ec7211">
  <img src="https://img.shields.io/badge/Amazon S3-232f3e?style=for-the-badge&logo=Amazon S3&logoColor=ec7211">
  <img src="https://img.shields.io/badge/Amazon RDS-232f3e?style=for-the-badge&logo=Amazon RDS&logoColor=ec7211"> <br>
  <img src="https://img.shields.io/badge/Github Actions-3373EF?style=for-the-badge&logo=Github Actions&logoColor=white"> <br>
<img src="https://img.shields.io/badge/KakaoAPI-FFCD00?style=for-the-badge&logo=&logoColor=black"> 

</div>

___
### 목차
<!-- TOC -->
- [새모임 프로젝트🕊️](#새모임-프로젝트️)
    - [프로젝트 설명 ](#프로젝트-설명-)
    - [기술 스택](#기술-스택)
    - [목차](#목차)
    - [프로젝트 개발 환경](#프로젝트-개발-환경)
    - [와이어 프레임](#와이어-프레임)
    - [서비스 아키텍처](#서비스-아키텍처)
    - [Class UML](#class-uml)
    - [ERD](#erd)
    - [API 문서](#api-문서)
    - [팀소개](#팀소개)
<!-- TOC -->
___
### 프로젝트 개발 환경
- spring-boot 3.0.2
- JDK 17
- build.gradle
<details><summary> 의존 주입
</summary>
<blockquote>
dependencies {

    implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
    implementation 'org.springframework.boot:spring-boot-starter-web'
    implementation 'org.springframework.boot:spring-boot-starter-validation'
    implementation 'org.springframework.boot:spring-boot-starter-security'

    compileOnly 'org.projectlombok:lombok'
    annotationProcessor 'org.projectlombok:lombok'

    testImplementation 'org.springframework.boot:spring-boot-starter-test'
    testImplementation 'org.springframework.security:spring-security-test'

    testCompileOnly 'org.projectlombok:lombok'
    testAnnotationProcessor 'org.projectlombok:lombok'

    compileOnly group: 'io.jsonwebtoken', name: 'jjwt-api', version: '0.11.2'
    runtimeOnly group: 'io.jsonwebtoken', name: 'jjwt-impl', version: '0.11.2'
    runtimeOnly group: 'io.jsonwebtoken', name: 'jjwt-jackson', version: '0.11.2'

    implementation 'mysql:mysql-connector-java'
    implementation 'com.google.code.gson:gson:2.9.0'

    implementation 'org.springframework.boot:spring-boot-starter-data-redis'

    implementation 'org.springframework.boot:spring-boot-starter-mail'

    implementation group: 'com.amazonaws', name: 'aws-java-sdk-s3', version: '1.12.410'
    implementation group: 'org.springframework.cloud', name: 'spring-cloud-starter-aws', version: '2.2.1.RELEASE'

    developmentOnly 'org.springframework.boot:spring-boot-devtools'
}
</blockquote>
</details>

___
### 와이어 프레임
<details><summary> wireFrame
</summary>
<img src="src/main/documents/wireFrame.png">
<img src="src/main/documents/wireFrame_02.png">
</details>

___

### 서비스 아키텍처
<details><summary> 서비스 아키텍처
</summary>
<img src="src/main/documents/serviceArchitecture.png">
</details>  

___

### Class UML

<details><summary>UML
</summary>
<img src="src/main/documents/classUML.png">
</details>

### ERD
<details><summary> ERD
</summary><img src="src/main/documents/ERD.png">
</details>

### API 문서
[새모임 API명세](https://d1axe8zrfcr62g.cloudfront.net/resources/static/docs/api-doc.html)

___
### 팀소개 

| 역할  | 이름 | 담당업무                                                                                                                                                                                              | 블로그                         |
|-----|----|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------|
| `리더`  | 이송언 | - 모임CRUD<br/>- 모임 참여 시스템<br/> - 모임 탈퇴<br/>- 모임 검색<br/> - 모임 위시리스트<br/> - 모임 리뷰CRUD<br/> - 비밀번호 찾기<br/> - 프로필CRUD<br/> - RESTDocs                                                                  | https://velog.io/@8essong30 |
| `부리더` | 장성준 | - JWT 토큰<br/> - 토큰 재발급<br/> - 스프링시큐리티<br/> - 로그인 및 로그아웃<br/> - 카테고리CRUD<br/> - 블랙리스트CRUD<br/> - 이메일 발송 기능<br/> - 인기모임조회<br/> - 신고하기CRUD<br/> - 회원 탈퇴<br/> - 카카오 로그인<br/> - 지도 API 연결<br/> - CI/CD | https://ace-jun.tistory.com |
| `팀원`  | 이지섭 | - 전체 프론트 구현 <br/> - 전체 프론트 동작 검수<br/> - 실시간 채팅 구현 <br/> - 채팅 저장/불러오기<br/> - 게시판 페이징                                                                                                               | https://velog.io/@leejiseop |
| `팀원`  | 김현중 | - 스프링 시큐리티<br/> - 회원가입 및 로그인<br/> - 게시판 CRUD<br/> - 좋아요기능<br/> - S3 이미지 구현 및 연결<br/>                                                                                                              | https://pooca12.tistory.com |
