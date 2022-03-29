<template >
  <div>
     <!-- Header nav  -->
   <nav class="header-nav">
     <!-- Logo -->
     <a href="#" class="header-nav-logo"><img src="../photos/logo.png" alt="Logo"></a>
     <ul class="nav-list">
       <li class="nav-item"><a href="#Work" class="nav-link">Work</a></li>
       <li class="nav-item"><a href="#About" class="nav-link">About</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Shop</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Blog</a></li>
       <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
     </ul>
     <!-- Hamburger icon -->
     <div class="nav-cart">
       <h1 class="nav-cart-title" @click="cart++">Cart({{cart}})</h1>
       <div class="nav-cart-hamburger" @click="togglebox" >
         <div class="hamburger-line"></div>
         <div class="hamburger-line"></div>
       </div>
     </div>
    </nav>
       <nav class="header-side-bar" v-if="sideBox">
         <a href="#" class="side-bar"><img src="../photos/logo.png" alt="Logo"></a>
         <div class="side-bar__close" @click="togglebox">
           <div class="sidebar-close__line line1"></div>
           <div class="sidebar-close__line line2"></div>
         </div>
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
  data() {
    return {
      sideBox:false
    }
  },
  props: {
    cart : {
      type : Number,
    },
  },

  methods: {
    togglebox() {
      this.sideBox = !this.sideBox
    }
  },
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
  scroll-behavior: smooth;
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
    background-color: #010032;
    width: 60%;
    height: 100%;
    margin-left: auto;
    transition: all .4s ease-in-out;
    cursor: pointer;
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
      margin-top: 6px;
      cursor: pointer;
      z-index: 999;
    }
  .side-bar__close {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
  }
    .sidebar-close__line {
      width: 41px;
      height: 3px;
      background: #ffff;
      cursor: pointer;
      z-index: 999;
    }
    .line1{
      transform: rotate(45deg);
    }
    .line2 {
      transform: rotate(-45deg);
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

    /* Media responsive */


    @media only screen and (max-width: 1200px) {}
    @media only screen and (max-width: 992px) {
      .nav-list  {
        display: none;
      }
    }
    @media only screen and (max-width: 768px) {
      .header-side-bar {
        width: 100%;
      }
    }
    @media only screen and (max-width: 576px) {}
    

</style>