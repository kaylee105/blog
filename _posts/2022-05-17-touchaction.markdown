---
title: "CSS touch-action"
layout: post
date: 2022-05-17 09:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- it
- 퍼블리셔
- 퍼블리싱
- css
- touch-action
category: blog
author: kaylee
star: true
description: it 퍼블리셔 퍼블리싱 csstouch-action
---

# CSS touch-action



### touch-action: 브라우저에게 맡길 터치 액션 지정

터치 이벤트의 처리는 브라우저가 담당하는 영역이다. Touch-action 속성을 통하여 요소 내에서 브라우저가 처리할 터치 액션의 목록을 지정할 수 있다.

터치를 사용한 스크롤(paning)과 여러 손가락을 사용한 확대/축소(pinch zoom)가 존재한다.

```css
/* 기본 값, 모든 터치 이벤트를 활성화 */
touch-action: auto;
/* 기본 값, 모든 터치 이벤트를 비활성화 */
touch-action: none;

/* 특정 축으로의 터치를 사용한 스크롤 허용 */
touch-action: pan-x;
touch-action: pan-y;

/* 특정 방향으로의 터치를 사용한 스크롤 허용 */
touch-action: pan-left;
touch-action: pan-right;
touch-action: pan-up;
touch-action: pan-down;

/* 핀치 줌(여러 손가락을 사용한 확대/축소)만 허용 */
touch-action: pinch-zoom;

/* 터치를 사용한 스크롤, 핀치 줌만 허용하고 그 외 비표준 동작 (더블 탭으로 확대 등) 불허용 */
touch-action: manipulation;

/* 동시에 여러 값 지정 가능 */
touch-action: pan-y pinch-zoom; 
```

[codepen](http://code.d2.co.kr/kaylee/220517.html)



## +

IOS 접근성 문제로 인해 meta 태그에 `user-scalable=no`를 추가하여도 사용자 휴대폰 설정에 확대/축소 가능으로 되어있다면 이를 제한할 수 없게 되었습니다.

이 때   `touch-action: pan-y ` 를 사용하면 확대/축소를 제한하고 세로 스크롤을 유지할 수 있습니다.
