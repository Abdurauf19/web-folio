<template >
<div class="main-port-img">
    <div class="main-portfolio-imgbox">
      <img :src="img" alt="portfolio img">
      <div class="portfolio-imgbox__content">
        <h3 class="imgbox__content__title">{{title}} </h3>
        <p class="imgbox__content__text">{{text}}</p>
      </div>
      <button class="img-box__btn">{{btn}}</button>
    </div>

    </div>
    
</template>

<script>
export default {
  props : {
    title:{
      type: String
      },
      text:{
        type:String
      },
      img: {
        type: String,
      },
      btn: {
        type: String,
      }
  }
}
</script>


<style >
    .main-port-img {
      float: right;
      padding: 0 40px 101px 60px;

    }


  .imgbox__content__title {
    font-size: 24px;
    line-height: 30px;
    font-family: var(--font_E);
    padding: 32px 0 23px 0;
    color: var(--titlee-color);
  }

  .imgbox__content__text {
    font-size: 12px;
    line-height: 28px;
    font-family: var(--font_E);
    max-width: 500px;
    color: var(--textt-color);
  }
  .img-box__btn {
    font-size: 16px;
    line-height: 24px;
    font-family: var(--font_E);
    background-color: var(--blue-color);
    color: #FFFF;
    padding: 40px 56px;
    max-width: 174px;
  }

  @media only screen and (max-with:1400px){
    
  }
   @media only screen and (max-width: 1200px) {
     .main-port-img {
      padding: 0 0px 101px 34px;
     }
   }
    
  
  @media only screen and (max-width: 992px) {
    .main-port-img {
      float: unset;
    }
  }
  @media only screen and (max-width: 768px) {
    .main-port-img {
      padding: 0 0 101px 0px;
    }

      .main-portfolio-imgbox img{
      width: 100%;
    }
  }
  @media only screen and (max-width: 576px) {
    .main-portfolio-imgbox img{
      width: 100%;
    }
  }
  @media only screen and (max-width: 320px) {
    .main-portfolio-imgbox img{
      width: 100%;
    }
  }
    
  
</style>