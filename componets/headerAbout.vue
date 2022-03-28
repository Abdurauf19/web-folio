<template>
  <div>
      <main class="main">
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
          <div class="expirence-number">
              <h3 class="expirence-number-num">{{Num}}</h3>
              <p class="expirence-number-text">{{Text}}</p>
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
  display: none;
  align-items: center;
  justify-content: center;
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

</style>


  
