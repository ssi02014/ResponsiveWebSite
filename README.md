# 💻 ResponsiveWebSite

### HTML, CSS, JS(Jquery)를 이용해서 만든 W3C 웹 표준 준수 반응형 사이트
### ⭐ Github Page : https://ssi02014.github.io/ResponsiveWebSite/

<br />
<br />

## 🎥 웹 페이지 화면 

![1](https://user-images.githubusercontent.com/64779472/93800827-1cf23100-fc7c-11ea-9ca9-eea5d11964ab.PNG)

![2](https://user-images.githubusercontent.com/64779472/93800831-1e235e00-fc7c-11ea-8e42-9ca348962595.PNG)

<br />
<hr />
<br />

## 🎥 W3C Check

![3](https://user-images.githubusercontent.com/64779472/93802630-ae62a280-fc7e-11ea-998c-e6e400129fbd.PNG)

<hr />

![4](https://user-images.githubusercontent.com/64779472/93802634-aefb3900-fc7e-11ea-9031-a88ecf316943.PNG)

<br />
<hr />
<br />

## 🔖 Main Development Stack
### 👨🏻‍💻 FrontEnd
1. HTML
2. CSS
3. JavaScript(Jquery)

<br />
<br />

## 📈 HTML 관련 학습 내용 또는 이슈
### 🔍 1. favicon 적용
```html
  <!-- 파비콘 -->
    <link rel="shortcut icon" href="icon/favicon.ico">
    <link rel="apple-touch-icon-precomposed" href="icon/favicon-152.png">
    <link rel="icon" href="path/to/favicon.png">
    <link rel="icon" href="icon/favicon-16.png" sizes="16x16"> 
    <link rel="icon" href="icon/favicon-32.png" sizes="32x32"> 
    <link rel="icon" href="icon/favicon-48.png" sizes="48x48"> 
    <link rel="icon" href="icon/favicon-64.png" sizes="64x64"> 
    <link rel="icon" href="icon/favicon-128.png" sizes="128x128">
```

<br />

### 🔍 2. 시맨틱 태그 
```html
  1. <header></header>: 헤더
  2. <nav></nav>: 네비게이션
  3. <aside></aside>: 사이드에 위치하는 공간
  4. <section></section>: 본문의 여러 내용(article)을 포함하는 공간
  5. <article></article>: 본문의 주 내용이 들어가는 공간
  6. <footer></footer>: 푸터
```

<br />

### 🔍 2. 반응형 이미지
```html
  반응형 이미지: 해상도, 스크린 크기 등이 다른 수많은 기기들에서 정상적으로 표시되는 이미지
  
  <!-- 반응형 이미지 사용 예시 -->
  <img 
    src="img/blog3_@1.jpg" 
    srcset="img/blog3_@1.jpg 1x, img/blog3_@2.jpg 2x, img/blog3_@3.jpg 3x" 
    alt="image" 
  />
```

<br />

### 🔍 3. Youtube 영상 가져오기
```html
  <!-- Youtube 영상 가져오기 사용 예시 -->
  <iframe 
    src="https://www.youtube.com/embed/dPRtcRwKo-Y?list=PLuHgQVnccGMBB348PWRN0fREzYcYgFybf" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen
  ></iframe>
```

<br />
<br />

## 📈 CSS 관련 학습 내용 또는 이슈
### 🔍 1. @media(미디어 쿼리)
```css
  /* 화면 너비 0 ~ 1220px : 데스크탑 */
  @media (max-width:1220px) {
    ...
  }
  /* 화면 너비 0 ~ 960px : 타블렛1 */
  @media (max-width:960px) { 
    ...
  }

  /* 화면 너비 0 ~ 768px : 타블렛2 */
  @media (max-width:768px){
    ...
  }

  /* 화면 너비 0 ~ 600px : 모바일1 */
  @media (max-width:600px){ 
    ...
  }

  /* 화면 너비 0 ~ 480px : 모바일2 */ 
  @media (max-width:510px){
    ...
  } 
  /* 화면 너비 0 ~ 360px : 모바일3 */ 
  @media (max-width:320px){ 
    ...
  }
```

<br />

### 🔍 2. 라이트 박스 이미지 효과
```css
  .square a:nth-child(1):hover img {filter: blur(2px);}
  .square a:nth-child(2):hover img {filter: brightness(50%);}
  .square a:nth-child(3):hover img {filter: contrast(10%);}
  .square a:nth-child(4):hover img {filter: grayscale(100%);}
  .square a:nth-child(5):hover img {filter: hue-rotate(120deg);}
  .square a:nth-child(6):hover img {filter: invert(100%);}
  .square a:nth-child(7):hover img {filter: opacity(10%);}
  .square a:nth-child(8):hover img {filter: saturate(10%);}
  .square a:nth-child(9):hover img {filter: sepia(120%);}
  .square a:nth-child(10):hover img {filter: sepia(120%) hue-rotate(120deg);}
```

<br />
<br />

## 📈 JavaScript 라이브러리(Jquery)
### 🔍 1. Slick을 이용한 Slide 구현하기
```html
  <!-- css insert -->
  <link rel="stylesheet" href="css/slick.css">

  <!-- script insert -->
  <script src="js/jquery.min_1.12.4.js"></script>
  <script src="js/slick.min.js"></script>
```

```javascript
  // jquery code
  $(".slider").slick({
      dots: true,
      autoplay: true,
      autoplaySpeed: 3000,
      arrows: true,
      responsive: [
          {
              breakpoint: 768,
              settings: {
                  autoplay : false
                  }
          }
      ]
  });
```

<br />

### 🔍 2. lightgallery를 이용한 gallery 구현하기
```html
  <!-- css insert -->
  <link rel="stylesheet" href="css/lightgallery.css">

  <!-- script insert -->
  <script src="js/lightgallery.min.js"></script>

  <!--light box-->
  <div class="lightbox square clearfix">
    <a href="img/light01_s.jpg">
        <img src="img/light01.jpg" alt="이미지">
        <em>blur</em>
    </a>
    <a href="img/light02_s.jpg">
        <img src="img/light02.jpg" alt="이미지">
        <em>brightness</em>
    </a>
    <a href="img/light03_s.jpg">
        <img src="img/light03.jpg" alt="이미지">
        <em>contrast</em>
    </a>
    <a href="img/light04_s.jpg">
        <img src="img/light04.jpg" alt="이미지">
        <em>grayscale</em>
    </a>
    <a href="img/light05_s.jpg">
        <img src="img/light05.jpg" alt="이미지">
        <em>hur-rotate</em>
    </a>
    <a href="img/light06_s.jpg">
        <img src="img/light06.jpg" alt="이미지">
        <em>invert</em>
    </a>
    <a href="img/light07_s.jpg">
        <img src="img/light07.jpg" alt="이미지">
        <em>opacity</em>
    </a>
    <a href="img/light08_s.jpg">
        <img src="img/light08.jpg" alt="이미지">
        <em>saturate</em>
    </a>
    <a href="img/light09_s.jpg">
        <img src="img/light09.jpg" alt="이미지">
        <em>sepia</em>
    </a>
    <a href="img/light10_s.jpg">
        <img src="img/light10.jpg" alt="이미지">
        <em>Mix</em>
    </a>
  <div class="lightbox square clearfix">
``` 

```javascript
  //jquery code
  $(".lightbox").lightGallery({
    ...
  });
```

<br />


