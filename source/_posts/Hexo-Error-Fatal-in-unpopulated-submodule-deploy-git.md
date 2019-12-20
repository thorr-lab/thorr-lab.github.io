---
title: '[Hexo, Error] Fatal: in unpopulated submodule .deploy_git'
layout: post
date: 2019-12-20 09:22:41
comments: true
tags: [Hexo, Error, hexo-deployer-git]
categories: [Hexo]
description: 
photos: 
  - https://feel5ny.github.io/images/post_img/01/thumb_default.jpg
---

### Hexo Blog 배포시 발생할 수 있는 에러
<img src="https://i.ibb.co/1fmH5vf/Hexo-Error.png" alt="Hexo-Error" border="0" style="max-width=100%; height: auto"><br>

이 에러가 발생한 배경을 보자면, 집 컴퓨터에서 배포, 밖에 나와서 내 노트북으로 받아와서 새로 배포하다가 발생한 문제입니다.

서로 다른 환경에서 배포를 하다보니 deploy 될 때 달라서 발생한 문제라고 생각됩니다.
해결방법은 간단합니다.

### 해결방법
``` shell
$ rm -rf .deploy.git
$ hexo g --d
```

감사합니다.