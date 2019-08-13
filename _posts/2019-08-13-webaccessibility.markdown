---
title: "Web Accessibility"
layout: post
date: 2019-08-13 21:09
image: /assets/images/markdown.jpg
headerImage: false
tag:
- web accessibility
- 웹 접근성
category: blog
author: Kaylee
description: 웹 접근성(web accessibility)
---
# 웹 접근성(**web** accessibility)



## 웹 접근성의 이해

#### 웹 접근성이란? 

어떠한 사용자(장애인, 노인 등), 어떠한 기술환경에서도 사용자가 전문적인 능력 없이 웹 사이트에서 제공하는 모든 정보에 접근할 수 있도록 보장하는 것으로 **특정 대상에 한정되지 않고** 모든 사용자를 대상으로 유익하게 하는것이 목적입니다. 

#### 웹 접근성의 필요성

- 누구에게나 동등한 기회 제공을 위해 웹 접근성 준수 필요
- 웹 접근성 보장은 법률에 명시된 의무사항

![](<https://code.d2.co.kr/kaylee/study/websoul.PNG>)



## 웹 접근성 지침

1. **이미지(그림, 사진, 로고, 차트, 다이어그램, 배경처리된 이미지, 동적으로 제공하는 이미지, 플래시의 Name값 등)에 적절한 대체 텍스트를 제공하는가?**

   - 전맹, 저시력의 경우 스크린리더나 점자정보단말기, 모바일의 VoiceOver, TalkBack 등을 활용하여 화면을 읽음. 태그내 alt속성의 값을 읽어주기때문에 alt속성을 제공하지 않으면 파일명을 읽어주어 어떤 이미지 인지 알수없기에 반드시 alt속성을 제공해야함. 또한 이미지와 최대한 동일한 내용으로 제공해주어야하고 의미없는 불릿이나 아이콘등의 이미지에는 alt속성을 빈값으로 제공해야함.

     ### **사례**

   ![](<https://code.d2.co.kr/kaylee/study/web1.jpg>)

   ![](<https://code.d2.co.kr/kaylee/study/web2.jpg>)

   

2. **포커스가 논리적인 순서로 이동하는가?**

   - 포커스 이동만으로 웹을 탐색할 때 모든 요소에 논리적인 순서(위→ 아래, 왼쪽 → 오른쪽, 메뉴 → 내용 등)로 접근 가능해야 하며, 포커스가 같은 영역에서 맴돌거나 더 이상의 이동이 어려운 경우가 발생하지 않도록 해야 함.

     ### 사례

     ![](<https://code.d2.co.kr/kaylee/study/web3.jpg>)

     

3. **포커스를 시각적으로 구별할 수 있는가?**

   - this.blur()나 outline:none 스타일을 지정하여 브라우저에서 기본적으로 제공되는 포커스 표시를 없애지 않도록 함.

     ### 사례

     ![](<https://code.d2.co.kr/kaylee/study/web4.PNG>)

4. W3C Validation을 통과하는가?

5. <table에 <caption이 적절하게 선언되었는가?

6. <thead,<tbody,<tfoot으로 그룹핑 되어 있는가? (th로 그룹핑 안될경우 <thead생략가능, tbody만 있을 경우 <tbody생략 가능)
    

7. 표의 머릿글은 <th>로 마크업 했으며 scope 속성을 제공하는가?

8. HTML 코드에 주언어 관련 속성(lang)이 선언되어 있는가?

9. 주요 콘텐츠 블록의 제목을 <h1>~<h6>로 마크업했는가?

10. 폼 콘트롤 요소에는 적절한 label을 제공하며, 폼 콘트롤 요소의 id값과 <label>의 for값을 동일하게 제공하는가?

    

## 접근성 평가도구

1. **N-WAX**
   ![](<https://code.d2.co.kr/kaylee/study/web6.png>)

![](<https://code.d2.co.kr/kaylee/study/web5.PNG>)



2. **모바일 스크린리더(ios/안드로이드)**

![](<https://code.d2.co.kr/kaylee/study/web7.PNG>)

3. UIA Varify
   플래시, 실버라이트 등 애플리케이션의 접근성 정보를 탐색할 수 있는 도구
4. PEAT
   웹 콘텐츠를 포함해서 스크린에 나타나는 대상이 발작 위험을 일으키는지 식별하는 도구
5. Contrast Ratio
   포토샵에서 전경색과 배경색의 명도 차이를 비교 할 수 있게 도와주는 확장 프로그램
6. 웹 브라우저 개발자 도구
   웹 콘텐츠 구성 요소를 탐색할 수 있으며 인터넷 익스플로러 외에도 대부분 브라우저가 지원



## 웹 접근성 품질 인증 

국가공인 웹 접근성 품질인증기관은 `한국웹접근성인증평가원(사단법인 한국장애인단체총연합회)`, `웹와치`, `사단법인 한국시각장애인연합회(한국웹접근성평가센터)`로 총 3개 기관을 지정

#### 인증현황

<https://www.wah.or.kr:444/Accessibility/auth.asp>



##### 참고

[웹 접근성 연구소](https://www.wah.or.kr:444/)
[NULI](https://nuli.navercorp.com/sharing/a11y)
