<template>
  <div>
      <main class="main" id="About">
    <div class="container about-container">
        <div class="main-about">
          <div class="main-about-comment">
              <img src="../photos/icon.png" alt="icon">
              <h3 class="about-comment-title">About</h3>
          </div>
          <div class="about-comment">
            <img src="../photos/stars.png" alt="stars">
              <p class="about-comment-ttext">{{About}}</p>
          </div>
          <div class="comment-user">
            <img src="../photos/UserPhoto.png" alt="userPhoto">
            <div class="user-content">
              <h3 class="user-content-name">Steve McQuillen</h3>
              <p class="user-content-job">CEO @ Vencortex</p>
            </div>
          </div>
        </div>
        <div class="main-expirience">
          <h2 class="main-expirence-title">Trusted by the fastest growing digital startups</h2>
          <div class="expirence-boxx">
          <div class="expirence-number">
              <h3 class="expirence-number-num">{{Num}}</h3>
              <p class="expirence-number-text">{{Text}}</p>
        </div>
          <div class="expirence-number">
              <h3 class="expirence-number-num">{{Num}}</h3>
              <p class="expirence-number-text">{{Text}}</p>
        </div>
          <div class="expirence-number">
              <h3 class="expirence-number-num">{{Num}}</h3>
              <p class="expirence-number-text">{{Text}}</p>
        </div>
          </div>
          <div class="expirence-images">
            <img src="../photos/logo/logo1.png" alt="Logo1">
            <img src="../photos/logo/logo2.png" alt="Logo2">
            <img src="../photos/logo/logo3.png" alt="Logo3">
            <img src="../photos/logo/logo4.png" alt="Logo4">
          </div>
        </div>
    </div>
      </main>
  </div>
</template>

<script>
export default {
  props: {
    About: {
      type:String ,
    },
    Num: {
      type:String,
    },
    Text: {
      type:String,
    },
  },
};
</script>

<style >
@import url('../public/font');

/* Fonts */
:root{
  --font_E:"Epilogue";
  --font_S:"SpaceGrotesk"
}
/* Colors */
:root {
  --titlee-color:#000000;
  --textt-color:#000000;
  --blue-color:#4543E8;
}
/* About comment Start */
.about-container {
  padding-top: 146px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 41px;
  padding-bottom: 200px;
}
  .main-about-comment {
    display: flex;
    align-items: center;
    column-gap: 20px;
    padding-bottom: 115px;
    
  }
  .about-comment-title {
    font-family:var(--font_E);
    font-size: 1rem;
    line-height: 1.5rem;
    letter-spacing: 2px;
    text-transform:uppercase;
    color:var(--blue-color);
  }

  .about-comment-ttext {
    color: var(--textt-color);
    font-family: var(--font_E);
    font-size: 1.18rem;
    line-height: 1.75rem;
    max-width: 24.4375rem;
  }

  .comment-user {
    display: flex;
    align-items: center;
   column-gap: 1.5rem;
   padding-top: 27px;
  }
  .user-content-name {
     font-size: 1.125em;
   color: var(--textt-color);
   font-family: var(--font_E);
   line-height: 1.5rem;
   margin: 0;
  }
  .user-content-job {
    font-family: var(--font_E);
    color: var(--textt-color);
    font-size: 0.9375rem;
    line-height: 1.5rem;
    margin: 7px 0 0 0 ;
  }

  /* expirence start */
.expirence-boxx {
  display: flex;
  gap: 64px;
}

.main-expirence-title {
  color: var(--titlee-color);
  font-family: var(--font_E);
  font-size: 3rem;
  max-width: 47.9375rem;
  line-height: 3.375rem;
  margin: 0 0 4.59rem 0;
}
/* expirence */
.expirence-number-num {
  color: var(--blue-color);
  font-family: var(--font_E);
  font-size: 3.75rem;
  line-height: 4.125rem;
  margin: 0;
}

.expirence-number-text{
  font-family: var(--font_E);
  color:var(--textt-color);
  font-size: 1.31rem;
  line-height: 1.9375rem;
  margin: 0;
}
/* Images  */
.expirence-images {
  display: flex;
  justify-content: center;
  padding-top: 72px;
  gap: 65px;
}

/* Media start */

@media only screen and (max-width: 1200px) {
.expirence-images {
  flex-wrap: wrap;
}
.expirence-boxx {
  flex-wrap: wrap;
  justify-content: center
}
}
@media only screen and (max-width: 992px) {

}
@media only screen and (max-width: 768px) {
.about-container {
  flex-direction: column;
  align-items: unset;
}
}
@media only screen and (max-width: 576px) {
.main-expirence-title {
  font-size: 2.4rem;
}
}

@media only screen and (max-width: 320px){
  
}
</style>


  
