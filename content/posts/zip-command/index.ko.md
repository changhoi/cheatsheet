---
title: 우분투 zip, unzip 하기
date: 2023-07-22
categories:
  - linux

tags:
  - linux
  - ubuntu
---

## zip, unzip

압축 하고 푸는 것을 도와주는 프로그램인데, 설치되어있지 않은 우분투에서는 아래 명령어로 설치할 수 있다.

<!--more-->

```bash
$ sudo apt-get install zip unzip
```

## zip 하는 방법

```bash
$ zip [압축파일 이름].zip [압축할 파일 or 디렉토리] [압축할 파일 or 디렉토리] ...

$ zip -r [압축파일 이름].zip [압축할 파일 or 디렉토리] ... # 디렉토리 압축

$ zip -j [압축파일 이름].zip [압축할 파일 or 디렉토리] ... # 디렉토리 이름 제외하고 압축

$ zip -u [압축파일 이름].zip [압축할 파일 or 디렉토리] ... # 변경되었거나 새로운 파일만 압축
```

ex.

```bash
$ zip Lambda-Deployment.zip ./* # 현재 폴더의 모든 파일을 Lambda-Deployment.zip으로 압축
```

## unzip 하는 방법

```bash
$ unzip [압축파일 이름].zip

$ unzip [압축파일 이름].zip -d [압축 푸는 위치] # 압축이 풀리는 위치를 특정할 수 있다.
```

## Reference

- <https://araikuma.tistory.com/120>
- <http://www.dreamy.pe.kr/zbxe/CodeClip/143985>
