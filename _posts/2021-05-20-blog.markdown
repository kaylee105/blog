
---
title: "Github 블로그 만들기"
layout: post
date: 2021-05-20 09:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- github
- blog
- Jekyll

category: blog
author: Kaylee
star: true
description: github,blog
---


# Github 블로그 만들기



## 저장소(repository) 만들기

Repositories에서 New클릭하면 새 저장소를 만드는 페이지가 나온다.{username}.github.io 형식으로 만들면 {username}.github.io 의 도메인으로 접속할 수 있는 블로그가 된다.



![img](http://code.d2.co.kr/kaylee/images/github)



## 테마 설정하기

Settings > pages >Theme Chooser > Choose a theme 

![img](http://code.d2.co.kr/kaylee/images/github2)

여기에서 몇가지 테마를 선택할 수 있다.

![img](http://code.d2.co.kr/kaylee/images/github3)

기본테마를 사용해도 문제 없지만, 

[https://jekyllthemes.io](https://jekyllthemes.io/) 에 디자인된 테마를 사용할 수 있다.

원하는 테마를 고른후 Github에서 zip파일로 다운받거나 clone 하는 방법이 있다.



#### zip파일로 다운받았을 시

- 다운 받은 테마의 모든파일을 {username}.github.io 디렉토리에 복사해 넣는다.

#### Clone 했을 경우

- github > settings 에서 Repository name을 {username}.github.io 으로 변경하면 쉽게 사용 할 수 있다.



![img](http://code.d2.co.kr/kaylee/images/github4)

{username}.github.io 접속후 적용이 잘되었는지 확인하면 된다:)



## 설정 변경하기

기본적인 설정은 _config.yml 파일에 있다. 이 외에는 테마에 따라 내용이 다르기 때문에 테마 제작자가 작성한 설명서를 확인해야한다.

![img](http://code.d2.co.kr/kaylee/images/github5)

이와 같이 기본적인 설정(블로그 제목/주소/설명 등등)을 변경할 수 있다



## `_posts` 에 새글쓰기

 `_posts` 폴더 생성후 `YYYY-MM-DD-post.md` 형식으로 포스트를 작성하면 된다.

이 형식은 Front matter라고 불리며, Jekyll글의 메타 데이터를 확인하여 준다. (테마 별로 다를수 있음)

포스팅시에 항상 상단에 적용하며, 테마별로 태그나 추가 정보를 변경할 수도 있다.

![img](http://code.d2.co.kr/kaylee/images/github6)

포스트 등록 완료:)

![img](http://code.d2.co.kr/kaylee/images/github7)



## 마치며..

Jekyll테마를 이용하여 블로그를 간편하게 만들 수 있으며, 원하는 레이아웃으로 변경도 가능하다.

포스팅시 마크다운 문법을 사용해야하지만, Typora 앱 또는 VScode 확장프로그램을 이용하면 되기 때문에 크게 어려운점은 없을 것 같다.





