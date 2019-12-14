---
title: "[CentOS 8]CentOS8에서 최신버전의 Nodejs 설치하기"
date: 2019-12-14 23:11:03
tags: [환경설정, nodejs, yum]
---

해당 내용은 아래의 링크 글을 참고해서 테스트를 진행하고 작성하였습니다. <br>
출처 : pizzu 님의 velog 글, [링크(클릭시 이동)](https://velog.io/@pizzu/centos-nodejs-%EC%B5%9C%EC%84%A0%EB%B2%84%EC%A0%84-%EC%84%A4%EC%B9%98%EB%B2%95)

---

### centos에서 yum 으로 nodejs 설치시 0.10.x 버전으로 설치가 되는 것을 최신 버전으로 받기위한 방법이다.


```shell
$ yum install -y gcc-c++ make     #의존성 패키지 설치
$ curl -sL https://rpm.nodesource.com/setup_8.x | sudo -E bash - #nodejs 최신버전 저장소 설치
$ yum install nodejs # nodejs 설치
```

### 버전 확인
<img src="https://i.ibb.co/9gdwsF1/version.png" alt="version" style="max-width:100%; height:auto;" border="0"/><br>

감사합니다.