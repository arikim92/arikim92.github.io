---
layout: post
comments: true
date: 2017-04-28 16:13:00
title: "리눅스 ln 명령어 (파일 참조)"
description: "관리자 권한이 필요한 파일을 참조해서 쉽게 수정하자"
subject: blog
categories: [ linux ]
tags: [ linux, ubuntu, nginx, copy ]
---

이 방법은 앞으로도 자주나오실 `Harrison Jung` 님께 전수(?)받은 방법입니다.

nginx 사용시에 설정할 때 마다 관리자 권한에, 터미널에, 수정하기 번거로우셨죠 ??? (저만인가요???)

복사하고 수정하시면 text 편집기에서 아주 쉽게 수정하실 수 있습니다.

좋으니 기분좋은 짤을 ( .. )

> 출처 Google / 네이버 대학일기 웹툰

<img src="https://scontent-ams3-1.cdninstagram.com/t51.2885-15/s640x640/sh0.08/e35/14156669_174188959657054_1410514566_n.jpg" alt="최재호 (@jaeho1130) Instagram media 2016-08-30 12:31:46" title="최재호 (@jaeho1130) Instagram media 2016-08-30 12:31:46 #포돌포돌동글동글#웹툰#대학일기웹툰" style="width: 200px;">

<br><br>

`ln -s` 를 사용하셔서 nginx 설정 파일들을 `/home/setting` 디렉토리에서도 사용할 수 있게 됩니다.

쉽게 설명하면 윈도우의 `바로가기` 를 생각하세요 !!

```bash
$ sudo su

$ ln -s /etc/nginx/nginx.conf
$ /home/setting/nginx.conf
$ ln -s /etc/nginx/sites-available/default
$ /home/setting/nginx_host.conf
```

> 나름 응용방법

`sublime text` 에서 `sftp` 를 이용합니다.

`/home/setting` 디렉토리로 연결합니다.

끝 !!

nginx 의 세계로 빠져봅니다 +_+
