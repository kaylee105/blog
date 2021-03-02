---
title: "반응형 웹(Responsive Web)"
layout: post
date: 2021-03-03 09:00
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
description: responsive web, Media Queries , viewport
---
# 반응형 웹(Responsive Web)



### 반응형 웹이란?

> 반응형 웹 디자인(Responsive Web Design)은 pc, 모바일, 태블릿 등 **각각의 기기별로**
> **홈페이지의 페이지가 최적화**되어 보여지는 기능. 화면이 작은 기기에서 반응형 웹으로 제작된 웹사이트를 접속했을 때 웹사이트의 구조를 작은 화면에 최적화된 구조로 변경하여 보여주고, 큰 화면을 가진 기기에서는 웹사이트의 구조를 큰 화면에 최적화된 구조로 변경하여 보여준다. 이처럼 **이용자 기기의 화면이나 환경에 맞게 자유자재로 변하는 것**이 반응형 웹입니다.



### 반응형 웹의 장점

1. 간편한 유지보수

   반응형 웹은 모바일, 태블릿, 데스크톱 등 모든 디자인을 하나의 HTML 파일과 CSS 파일에서 작업하기 때문에 유지 보수가 훨씬 쉽고 간편하다.

2. 마케팅

   언제, 어디서, 어떻게든 접근이 용이해야 하는 마케팅에 최적화된 웹 기술

3. 검색 엔진 최적화 (SEO(Search Engine Optimize)) 

   반응형 웹으로 만들어진 경우 하나의 주소와 하나의 파일로만 이루어져 검색 결과에 더 잘 노출될수 있고 광고효과를 볼수 있으며 광고비용도 절약할수있다.



------



## 뷰포트(viewport)

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

`width` 는 뷰포트의 가로크기를 지정한다. `device-width`일시 기기의 스크린 너비에 맞춘다는 뜻

| **width**              | 뷰포트의 가로 크기                                           |
| ---------------------- | ------------------------------------------------------------ |
| **initial-scale**      | 페이지 처음 접속시 보여질 배율                               |
| **user-scalable**      | 사용자의 축소/확대 허용 여부                                 |
| **minimum-scale**      | 뷰포트의 최소 배율 값 (0~10)                                 |
| **maximum-scale**      | 뷰포트의 최대 배율 값 (0~10)                                 |
| **viewport-fit=cover** | ios 가로모드시 자동 적용된 패딩을 제외하고 전체화면으로 사용(최적화) |



## 미디어쿼리(Media Queries)

1. css내에 직접 사용

```css
@media (max-width:768px) {}
```

2. <link>요소를 사용하여 조건이 맞을시에 css파일 로드

```html
<link rel="stylesheet" media="screen and (max-width: 768px)" href="mobile.css" />
```

3. style 태그내에 사용하며 midea속성 조건이 맞을시에 적용

```html
<style type="text/css" media="screen and (max-width: 768px">
 /* style */
</style>

<style>
    @import url(mobile.css) screen and (max-width: 768px);
</style>
```

### 구문

<img src="http://code.d2.co.kr/kaylee/study/media.png" alt="img">

미디어 쿼리 구문은 '미디어 타입 / 논리 연산자 / 속성' 으로 이루어진다.

##### 미디어 타입

| **all**    | 모든 미디어 타입                  |
| ---------- | --------------------------------- |
| **print**  | 인쇄 결과물 및 인쇄 미리보기 문서 |
| **screen** | 화면 대상                         |

##### 속성

| **width**       | 웹 페이지의 가로 길이                                        |
| --------------- | ------------------------------------------------------------ |
| **height**      | 웹 페이지의 세로 길이                                        |
| **orientation** | 뷰포트 방향(가로값이 더 클경우 landscape/세로값이 더 클경우 portrait) |
| **hover**       | 웹에서만 적용                                                |

##### 논리 연산자

| **and** | 모든 쿼리가 참이여야 적용     |
| ------- | ----------------------------- |
| **not** | 모든 쿼리가 거짓이여야 적용   |
| **,**   | 어느 하나라도 참이면 적용(or) |



### 모바일과 데스크탑, 우선순위

모바일과 데스크탑중 우선순위 정하기.

- 모바일 퍼스트일시 `min-width` 사용하여 분기점이 낮은 순서대로 작성

- 데스크탑일시 `max-width` 사용하여 분기점이 높은 순서대로 작성

```css
/* Mobile First */

.title { font-size: 12px; }
 
@media (min-width: 768px) {
  .title { font-size: 14px; }
}
@media (min-width: 1024px) {
  .title { font-size: 16px; }
}
@media (min-width: 1440px) {
  .title { font-size: 18px; }
}
```

```css
/* Desktop First */
 
.title { font-size: 18px; }
 
@media (max-width: 1440px) {
  .title { font-size: 16px; }
}
@media (max-width: 1024px) {
  .title { font-size: 14px; }
}
@media (max-width: 768px) {
  .title { font-size: 12px; }
}
```



## 가변형 레이아웃

사이트의 모든 요소를 상대적인 크기로 지정해서 브라우저 크기에 따라서 다르게 표시해주는 방법

### Flex

한 방향 레이아웃

### Grid

두 방향(가로-세로) 레이아웃

### Multi-column layout

다중 칼럼 레이아웃, 신문과 같이 여러 개의 칼럼으로 구성되는 구조



------



## 미디어쿼리 다양하게 사용하기



### mixin

```scss
// Break Point
$desktop: 1440px;
$tablet: 1024px;
$mobile: 768px;

// Mixins
@mixin desktop {
  @media (max-width: #{$desktop}) {
    @content;
  }
}

@mixin tablet {
  @media (max-width: #{$tablet}) {
    @content;
  }
}
 
@mixin mobile {
  @media (max-width: #{$mobile}) {
    @content;
  }
}
```

#### 중첩 미디어쿼리

```scss
.title {
  font-size: 20px;
}
 
/* 별도로 작성 */
@include tablet {
  .title {
    font-size: 16px;
  }
}
```

```scss
.title {
  font-size: 20px;
  
  /* 요소에 바로 작성 */
  @include tablet {
    font-size: 16px;
  }
}
```

요소에 바로 작성하는 경우 직관적이며 유지보수에 용이하지만 컴파일시 미디어 쿼리 구문이 계속 중복된다

이는 gulp를 이용하여 중복된 구문을 제거할수있다. 

[gulp-group-css-media-queries]: https://www.npmjs.com/package/gulp-group-css-media-queries

```javascript
var gulp = require('gulp');
var gcmq = require('gulp-group-css-media-queries');
 
gulp.task('default', function () {
    gulp.src('src/style.css')
        .pipe(gcmq())
        .pipe(gulp.dest('dist'));
});
```



### Viewport에 따른 가변 단위

브라우저 창의 너비나 높이에 따라 크기가 변하는 가변 폰트 단위 `vw` `vh` `vmin` `vmax`

| **vw** | Viewport width, 웹 브라우저의 가로폭을 기준으로 결정         |
| ------ | ------------------------------------------------------------ |
| **vh** | Viewport height, 웹 브라우저의 세로폭을 기준으로 결정        |
| vmin   | Viewport minimum, 웹 브라우저의 가로폭과 세로폭중에 더 작은 값을 기준으로 한다 |
| vmax   | Viewport maximum, 웹 브라우저의 가로폭과 세로폭중에 더 큰값을 기준으로 한다 |

[^Vmax]: IE11,Edge13,Edge14에서는 미지원



### em / rem

`em` '1em = 부모의 폰트 크기'

부모의 폰트 크기가 20px이라면 1em = 20px, 3em =60px으로 커지게 됨

[PXtoEM]: http://pxtoem.com/

```scss
$font-size: 16; 
 
@function em($pixels, $context: $font-size) {
  @return #{$pixels/$context}em;
}
 
.title {
  font-size: em(32); // 32/16 = 2em;
}
```

`rem` ' 1rem = html의 폰트 크기'

브라우저가 지정해주는 기본 폰트 사이즈는 `100% = 16px`

계산하기 쉽게 `62.5% = 10px` 으로 변경하면 `1rem = 10px` 로 사용할 수 있다.

```css
html { font-size: 62.5%; }

.image { width: 24rem; } //240px
.text { font-size: 1.6rem; } //16px
.desc { margin-top: 2rem; } //20px
 
@media all and (max-width: 768px) {
  html { font-size: 50%; }
}
```



### Case

1. 화면 크기에 따른 이미지 제어

   ```javascript
   $(window).resize(function() {
     if($(window).width() >768) {
       
     }
   });
   ```

   

2. 반응형으로 비디오 삽입하기

   ```html
   <div class="video">
       <div class="video-container">
         <iframe width="100%" height="100%" src="https://www.youtube.com/embed/eitDnP0_83k?controls=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
       </div>
   </div>
   ```

   ```css
   .video {
     width: 100%;
   }
    
   .video-container {
     position: relative;
     width: 100%;
     height: auto;
     padding-top: 56.25%; /* 영상 비율 16:9일 경우 */
   }
    
   iframe {
     z-index: 1;
     top: 0;
     left: 0;
     position: absolute;
     width: 100%;
     height: 100%;
   }
   ```

3. 모바일에서만 슬라이드 실행

   ```javascript
       if (window.innerWidth < 768) {
           $('.slick-slider').slick();
       }
       $(window).resize(function (e) {
           if (window.innerWidth < 768) {
               if (!$('.slick-slider').hasClass('slick-initialized')) {
                    $('.slick-slider').slick();
               }
           } else {
               if ($('.slick-slider').hasClass('slick-initialized')) {
                   $('.slick-slider').slick('unslick');
               }
           }
       });
   ```

   









참고

[vw, vh, vmin, vmax, em, rem 속성]: https://nykim.work/85

