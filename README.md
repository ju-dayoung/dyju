# SWIPER 패럴럭스 넘김 


## STEP01. 마크업

스와이퍼 슬라이드 마크업 
```
<div class="pallax-slide">
  <div class="swiper-wrapper">
    <div class="swiper-slide"><img src="./images/sld_01.jgp" alt=""></div>
    <div class="swiper-slide"><img src="./images/sld_02.jgp" alt=""></div>
    <div class="swiper-slide"><img src="./images/sld_03.jgp" alt=""></div>
  </div>
  <div class="swiper-pagination"></div>
  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>
</div>

```

## STEP02. swiper 설정

```
var mySwiper = new Swiper('.bannar .swiper-container', {
  navitation : {
    nextEl:'.swiper-button-next',
    prevEl:'.swiper-button-prev',
  },
  loop:true,
  direction:'horizontal',
  slidePerView:'auto',
  loop:true,
  spaceBetween:0,
  speed:800
});
```
