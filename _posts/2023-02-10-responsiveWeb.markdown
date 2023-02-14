---
title: "반응형 웹(Responsive Web)"
layout: post
date: 2023-02-10 21:09
image: /assets/images/markdown.jpg
headerImage: false
tag:
- responsive
- responsive Web
- viewport
- Media Queries
- vw
- em

category: blog
author: Kaylee
star: false
description: responsive web, Media Queries , viewport
---
# 반응형 웹(Responsive Web)



## 반응형 웹이란?

> 다양한 화면의 폭에 따라 유동적으로 레이아웃이 변화하는 웹



https://mediaqueri.es/



- 반응형웹 : 모든 화면에 하나의 템플릿으로 제작
- 적응형웹 : 지원할 디바이스(화면)에 따라 별도의 템플릿 제작



![img](https://blog.kakaocdn.net/dn/qW5iW/btqC9NQrbst/VUCG10F0KtElkx6QMxdkv1/img.gif)

반응형(Responsive)과 적응형(Adaptive)웹 차이



### 장점

1. 간편한 유지보수와 모니터링

   반응형 웹은 모바일, 태블릿, 데스크탑 등 모든 디자인을 **하나**의 HTML 파일과 CSS 파일에서 작업하기 때문에 유지 보수가 훨씬 쉽고 간편하다.

2. 디바이스 기기 호환성

   화면의 폭에 따라 유동적으로 레이아웃이 변경되기에 모든 디바이스 호환 가능하다.

3. 검색 엔진 최적화 (SEO(Search Engine Optimize))

   반응형 웹으로 만들어진 경우 하나의 주소와 하나의 파일로만 이루어져 검색 결과에 더 잘 노출될수 있고 광고효과를 볼수 있으며 광고비용도 절약할수있다.

   

### 단점

1. 콘텐츠 한계

   화면 크기나 사용자 디바이스에 따라 유동적으로 변하기 때문에 많은 내용이 들어가면 디자인 및 구현의 한계가 있다.

2. 로딩 속도

   너무 많은 콘텐츠를 불러오려면 로딩 속도가 길어지기 때문에 성능 이슈가 발생하며 이로 인한 사용자 이탈률이 증가할 수 있다.

3. 레이아웃 변경의 어려움

   기존에 제작한 레이아웃의 변경이 어렵다. 각 해상도 별 분기점을 기준으로 콘텐츠 위치를 잡아두기에 새로운 것을 추가하는 작업 공수가 크다.

   이러한 이유로 반응형 웹은 주로 정적인 회사소개 페이지나, 블로그 커뮤니티 등을 포함 할때 제작한다.

   

## 기획

1. #### 우선순위 관점 정의

   모바일과 데스크탑의 우선순위를 정한다.

   ![progressive enhancement](https://bradfrost.com/wp-content/uploads/2011/06/progressive_enhancement.jpg)

   데스크탑 환경에 맞춰 제작한 뒤 모바일 환경에 맞게 점진적으로 줄여나가는 것과

   모바일 환경에 맞춰 제작한 뒤 데스크탑에 맞게 점진적으로 향상시켜 나가는 것을 비교해 볼수 있다.

   방대한 정보를 담고있는 복잡한 레이아웃의 웹사이트는 모바일 사용자에게는 필요이상의 정보와 그에 따른 리딩 및 로딩 시간에 문제가 야기될수 있다.

   

2. #### 가변 단계 정의

   지원할 디바이스 사이즈의 범위를 정하고 그에 따른 가변 단계를 정의해야한다. 

   (보통 모바일,태블릿,웹 3단계로 구분한다.)

   

   + ##### 반응형이 일어나는 기준 (Breakpoints)

     현재 가장 많이 사용되는 PC,Tablet,Mobile 해상도이며 사이트에 맞는 기준을 정하면 된다.

     

     ![img](https://aws-code.d2.co.kr/kaylee/images/responsive.jpg)

   

3. #### UI 구성 요소 정의

   + 이미지 사이즈 규정 : 확대/축소, 행/열 조정
   + 폰트 사이즈 규정
   + 그리드 규정
   + 링크 규정 (새창을 통한 페이지이동,현재창 이동)
   + 터치 행위 고려

   

## 디자인

1. 유동형 그리드(fluid grids)

   고정된 px이 아닌 em이나 %를 사용한다.
   
   https://aws-code.d2.co.kr/kaylee/images/mio-design.mp4
   
   

2. 유연한 이미지(fluid/flexible images)

   유동형 그리드와 마찬가지로, 고정된 px이 아닌 em과 %를 이용하는 방법으로, max-width를 100%로, height를 auto로 설정하는 방법으로 화면 폭에 따라 가로/세로 길이가 줄었다 늘어나는 방법

   

   ![img](https://i0.wp.com/knulab.com/wp-content/uploads/2019/02/02_Relative-Units-vs-Static-Units-1.gif?resize=1100%2C400&ssl=1)

   

3. 반응형 레이아웃(responsive layouts)

   ![img](https://www.nextree.co.kr/content/images/2021/01/jsseo-140329-CSS-01-1024x415-1.png)

   

   

   + 부트스트랩 레이아웃

   https://colorlib.com//polygon/adminty/default/index.html

   

   + 머티리얼 디자인

   https://m2.material.io/design/layout/responsive-layout-grid.html#columns-gutters-and-margins



## 마치며

반응형 웹은 하나의 코드로 다양한 디바이스를 호환한다는 장점이 있지만, 그로인해 고려해야할 사항이 많습니다. 각 파트별로 반응형 웹에 대한 개념을 이해하고 반응형 웹이 주는 이점을 효율적으로 사용였으면 합니다.



------

* 참고사이트

https://uipac.com/45

https://hyoni-k.tistory.com/121

https://brunch.co.kr/@clay1987/134
