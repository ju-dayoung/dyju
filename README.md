# SWIPER 패럴럭스 넘김 


## STEP01. 마크업

스와이퍼 슬라이드 마크업 
```
<div class="parallax-slide swiper-container">
  <div class="swiper-wrapper">
    <div class="swiper-slide"><img src="./images/sld_01.jpg" alt=""></div>
    <div class="swiper-slide"><img src="./images/sld_02.jpg" alt=""></div>
    <div class="swiper-slide"><img src="./images/sld_03.jpg" alt=""></div>
  </div>
  <div class="swiper-pagination"></div>
  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>
</div>

```

## STEP02. swiper 설정

```
var mySwiper = new Swiper('.parallax-slide ', {
  navigation : {
    nextEl:'.swiper-button-next',
    prevEl:'.swiper-button-prev',
  },
  pagination:{
    el:'.parallax-slide .swiper-pagination',
    clickable: true,
  },
  loop:true,
  direction:'horizontal',
  slidePerView:'auto',
  loop:true,
  parallax:true, // 반드시 parallax:true설정.
  spaceBetween:0,
  speed:800
});
```

## STEP03. swiper-slide안의 element에 속성 추가

data-swiper-parallax 속성을 추가해야 한다.
```
<div class="swiper-slide">
  <img src="./images/sld_01.jpg" alt="" data-swiper-parallax="90%">
</div>
```

## STEP04. swiper-slide에 css 추가

```
.swiper-container { /* 여러 속성들.. */ overflow:hidden; }
```



