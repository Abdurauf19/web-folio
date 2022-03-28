<template >
  <div>
     <!-- Header nav  -->
   <nav class="header-nav">
     <!-- Logo -->
     <a href="#" class="header-nav-logo"><img src="../photos/logo.png" alt="Logo"></a>
     <ul class="nav-list">
       <li class="nav-item"><a href="#" class="nav-link">Work</a></li>
       <li class="nav-item"><a href="#" class="nav-link">About</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Shop</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Blog</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
     </ul>
     <!-- Hamburger icon -->
     <div class="nav-cart">
       <h1 class="nav-cart-title" @click="cart++">Cart({{cart}})</h1>
       <div class="nav-cart-hamburger">
         <div class="hamburger-line"></div>
         <div class="hamburger-line"></div>
       </div>
     </div>
    </nav>
       <nav class="header-side-bar">
         <a href="#" class="side-bar"><img src="../photos/logo.png" alt="Logo"></a>
         <ul class="side-bar-list">
           <li class="side-bar-item"><a href="#Work" class="side-bar-link">Work</a></li>
           <li class="side-bar-item"><a href="#About" class="side-bar-link">About</a></li>
           <li class="side-bar-item"><a href="#Shop" class="side-bar-link">Shop</a></li>
           <li class="side-bar-item"><a href="#Blog" class="side-bar-link">Blog</a></li>
           <li class="side-bar-item"><a href="#Contact" class="side-bar-link">Contact</a></li>
         </ul>
       </nav>
  </div>
</template>

<script>
export default {
  props: {
    cart : {
      type : Number,
    }
  }
}
</script>


<style scoped>
  
@import url("../public/font");
:root{
  --font_E:"Epilogue";
  --font_S:"SpaceGrotesk"
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

ul {
  list-style: none;
}
a{
  text-decoration: none;
}
  /* header start */
  .header-nav {
    background-color: #010032;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 100%;
    position: fixed;
    top:0;
  }
  .nav-list {
    display: flex;
    align-content: center;
    column-gap:40px;
  }
  .nav-cart {
    display: flex;
    align-items: center;
    gap: 15px;
  }

  /* Hamburger line */

  .header-side-bar {
    position: fixed;
    left: -100%;
    background-color: #010032;
    width: 50%;
    height: 600px;
    margin-left: auto;
  }
  .side-bar-list {
    display: flex;
    flex-direction:column;
    align-items: center;
    justify-content: space-around;
    row-gap: 30px;
  }
    .nav-cart h1 {
      color: #FFFFFF;
      font-family: var(--font_E);
      font-size: 15px;
      line-height: 19px;
    }
    .hamburger-line {
      width: 25px;
      height: 2px;
      background: #ffff;
      margin: 6px;
      cursor: pointer;
    }
    .header-nav img{
      margin: 28px 0 23px 0;
    }
    /* Header link */
    .nav-link, .side-bar-link{
      color: #ffff;
      font-family: var(--font_E);
      font-size:15px; 
      line-height: 19px;
      position: relative;
     transition: all .5s ease-in-out;
     opacity: 0.8;
    }
    .nav-link:hover {
      opacity: 1;
       border-bottom: 4px solid #e5e5eb;
    }
    .side-bar-link {
      position: static;
      border: 0;
    }
    

</style>