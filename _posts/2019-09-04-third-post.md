---
title: "[javaScript] 비동기적 javascript : 비동기 처리 방법"
categories:
  - Javascript
tags:
  - Javascript
---

자바스크립트는 하나의 스레드 (Single Thread) 기반의 언어  

자바스크립트 엔진 : memory Heap + single Call Stack  

자바스크립트 엔진만으로는 비동기성을 활용할 수 없다.  

- - -

* 자바스크립트 실행에 관여하는 요소
    * Web API ( 브라우저에서 제공되는 API )
        - DOM, AJAX, setTimeout
        - 비동기 작업을 실행 후 callback 을 task queue 에 넘겨줌
    * Task Queue ( Callback Queue )
        - Web API 에서 전달 받은 callback function 을 담고 있는 Queue
    * Event Loop
        - 자바스크립트 엔진의 call stack 이 비어있는 지 확인하고 task queue 의 callback을 call stack 에 넣어주는 역할

- - -

참고 URL : <https://hudi.kr/비동기적-javascript-싱글스레드-기반-js의-비동기-처리-방법/>