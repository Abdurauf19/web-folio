<template>
  <div>
    <div class="container" id="Work">
      <div class="main-portfolio">
        <div class="main-portfolio-titlee">
          <img src="../photos/icon.png" alt="icon">
          <h3 class="main-portfolio-textt">{{portfolioTitle}}</h3>
        </div>
        <h2 class="main-portfolio-title">{{portfolioText}}.</h2>
      </div>
    </div>
  </div>
</template>



<script>
export default {
  props:{
    portfolioTitle :{
      type:String,
    },
    portfolioText : {
      type:String,
    },

  }
}
</script>


<style>
body {
  scroll-behavior: smooth;
}
/* title work */
  .main-portfolio-titlee{
    display: flex;
    align-items: center;
    column-gap: 20px;
  }

  .main-portfolio-textt {
    font-family: var(--font_E);
    color: var(--blue-color);
    font-size: 16px;
    line-height: 24px;
    text-transform: uppercase;
  }

  .main-portfolio-title {
    font-family: var(--font_E);
    max-width: 698px;
    font-size: 60px;
    line-height: 66px;
    color: var(--titlee-color);
      padding: 26px 0 78px 0;
  }
</style>