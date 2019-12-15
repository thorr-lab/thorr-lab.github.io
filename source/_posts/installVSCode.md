---
title: "[CentOS 8]Centos8에 VSCode 설치하기"
layout: post
date: 2019-12-14 22:23:48
comments: true
tags: [환경설정, VSCode, yum]
categories: [Config CentOS8]
description: 
photos: 
  - https://i1.wp.com/gtbensmagazine.com/wp-content/uploads/2019/04/CentOS.png?w=600&ssl=1
---
<img src="https://i.ibb.co/LR3pfL4/image.png" alt="image" style="max-width: 100%; height:auto;" border="0" /><br>
원본 링크 : https://code.visualstudio.com/docs/setup/linux


### VS Code를 어떻게 설치하느냐?
1. key & repository 설치, yum repo로 안정적으로 설치하기 위해서 하는 준비 단계
```shell
$ sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
$ sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
```

*여기서 부터는 두가지 방법이 있는데 둘 중 하나 선택해서 편한걸로 하시면 됩니다.*

2. yum 으로 설치
```shell
yum check-update
sudo yum install code
```

3. dnf으로 설치
```shell
sudo dnf check-update
sudo dnf install code
```

**만약 dnf가 설치 되어 있지 않다면? ('yum으로 까세요'라고 말씀드리고 싶지만 아래와 같이 하면 된다고 합니다.)**
4. dnf 설치 -> 이후 3과정 다시 진행
```shell
wget http://springdale.math.ias.edu/data/puias/unsupported/7/x86_64/dnf-conf-0.6.4-2.sdl7.noarch.rpm
wget http://springdale.math.ias.edu/data/puias/unsupported/7/x86_64//dnf-0.6.4-2.sdl7.noarch.rpm
wget http://springdale.math.ias.edu/data/puias/unsupported/7/x86_64/python-dnf-0.6.4-2.sdl7.noarch.rpm
yum install python-dnf-0.6.4-2.sdl7.noarch.rpm  dnf-0.6.4-2.sdl7.noarch.rpm dnf-conf-0.6.4-2.sdl7.noarch.rpm
```

감사합니다. <br>