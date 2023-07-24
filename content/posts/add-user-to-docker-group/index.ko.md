---
title: 리눅스에서 Docker 명령어 sudo 없이 사용하기
date: 2023-06-22

categories:
  - linux
tags:
  - linux
  - ubuntu
  - docker
---

리눅스에서는 docker 명령어 앞에 항상 `sudo`를 붙여야 하는 불편함이 있었는데, 현재 계정을 docker 그룹에 추가하면 권한 문제가 해결된다. 방법은 아래와 같다.

```bash
sudo usermod -aG docker $USER
```
