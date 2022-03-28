<template>
  <div>
    <header class="header" id="Header">
      <div class="container header-container">
        <div class="heade-content">
          <h1 class="header-content-title">I design digital products that make an impact.</h1>
          <p class="header-content-text">Hi! Im Alex, a product designer based in Oakland. I create user-friendly interfaces for fast-growing startups.</p>
          <button class="header-content-btn btn">Hire me!</button>
        <div class="header-awards">
          <img src="../photos/awrds-icon.png" alt="awards">
          <div class="awards-content">
            <h3 class="awards-content-title">Independent Of The Year</h3>
            <p class="awards-content-text">Annual Awards 2020 • awwwards.com</p>
          </div>
        </div>
        </div>
        <div>
          <img src="../photos/header-banner.png" alt="header banner" class="header-img">
        </div>
      </div>
    </header>
    
  </div>
</template>


<script>
export default {
  props: {

  }
}
</script>

<style >
@import url('../public/font');

:root{
  --font_E:"Epilogue";
  --font_S:"SpaceGrotesk"
}
:root {
  --background-color:#010032;
  --title-color:#FFFF;
  --text-color:#ffff;
}
  /* Headet start */
    .header-container {
      display: flex;
      align-content: center;
      justify-content: center;
      background-color: var(--background-color);
    }

    .header-content-title {
      color: var(--title-color);
      font-family: var(--font_E);
      font-size: 4.5rem;
      line-height: 4.75rem;
      max-width: 604px;
    }

    .header-content-text {
      color: var(--text-color);
      font-family: var(--font_E);
      font-size: 1.37rem;
      line-height: 2.2rem;
      max-width: 542px;
    }

    .btn {
      color: #010032;
      background-color: #FFFF;
      padding: 21px 0;
      font-size: 18px;
      border-radius:32px;
      font-family: var(--font_E);
      width: 203px;
    }

    .header-awards {
      display: flex;
      align-items: center;
      padding-top: 100px;
      gap: 24px;
    }

    .awards-content-title {
      color: var(--title-color);
      font-family: var(--font_E);
      font-size: 18px;
      line-height: 26px;
    }
    .awards-content-text {
      color: var(--text-color);
      font-family: var(--font_E);
      font-size: 15px;
      line-height: 22px;
    }

</style>