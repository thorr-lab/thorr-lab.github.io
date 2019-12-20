---
title: "[Web] Web Server vs WAS"
date: 2019-12-19 18:59:40
tags: [Web, WAS]
layout: post
comments: true
categories: [Web Tech]
description: 
photos: 
  - https://gmlwjd9405.github.io/images/web/webserver-vs-was1.png
---


본 글은 아래 글을 보며 작성하였습니다.
출처 : https://gmlwjd9405.github.io/2018/10/27/webserver-vs-was.html

---

### WAS = Web Application Server

**Q: Web Server랑 동일한 것? <br>
A**: 다른 것

Web Server : 

- Web Server는 파일 경로의 이름을 받아 경로와 일치하는 FILE 을 반환한다.
- 이때 항상 동일한 페이지를 반환한다. 이를 Static Pages 라고 말함
- html, css, javascript 파일과 같이 파일에 컴퓨터에 저장되어 있는 파일들을 의미

WAS:

- DB 조회나 다양한 로직 처리를 요구하는 동적인 컨텐츠를 제공하기 위해 만들어진 Application Server
- 동적인 contents를 반환하는 기능을 한다. 이러한 기능을 하는 페이지를 Dynamic Pages

### 그래서 Web Server?

하드웨어적 정의 : Web 서버가 설치되어있는 컴퓨터

소프트웨어적 정의 : 웹 브라우저로부터 HTTP 요청을 받아 정적인 컴퓨터를 제공하는 컴퓨터 프로그램

### 기능

- HTTP 프로토콜을 기반으로 클라이언트의 요청을 서비스 하는 기능
    - 정적 콘텐츠 제공
- 동적인 컨텐츠 제공을 위한 요청 전달
    - 클라이언트의 요청 WAS에 전달, WAS가 처리한 결과를 클라이언트에 전달

### 예 :

Apache Server, Nginx, IIS 등..

### WAS(Web Application Server)

HTTP를 통해 컴퓨터나 장치에 어플리케이션을 수행해주는 미들웨어(소프트웨어 엔진)

### 기능

- WAS = Web Server + Web Container
- 프로그램 실행 환경 & DB 접속 기능 제공
- 여러 개의 트랜잭션 관리 기능
- 업무를 처리하는 비즈니스 로직 수행

### Web Container, Servlet Container :

- JSP, Servlet을 실행시킬 수 있는 소프트웨어

### 예 :

ex) Tomcat, JBoss, Jeus, Web Sphere

감사합니다.