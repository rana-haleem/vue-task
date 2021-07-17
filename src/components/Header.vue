<template>
  <header class="flex items-center">
      <div class="flex items-center logo-container">
          <img alt="prank logo" src="../assets/Logo.svg">
          <div class="flex items-center justify-center search-container"> 
            <img class="desktop" alt="search logo" src="../assets/search.svg">
          </div>
      </div>
      <div class="nav-links-dk flex items-center">
          <nav>
              <a>Prank Call Videos</a>
              <a>Prank Request </a>
              <a>Store</a>
              <a>Prank Apps</a>
              <a>Blog</a>
          </nav>
          <div class="flex stores"> 
              <div class="flex items-center"> 
                  <img src="../assets/applestore.svg" alt="apple store">
              </div>
               <div class="flex items-center"> 
                  <img src="../assets/playstore.svg" alt="play store">
              </div>
          </div>
          <div class="flex header-btns"> 
              <button class="login">login</button>
              <button class="sign-up">Sign up</button>
          </div>
      </div>
      <div class="burger-menu"> 
           <img class="mobile" alt="search logo" src="../assets/searchMob.svg">
            <Slide>
                <a>Prank Call Videos</a>
                <a>Prank Request </a>
                <a>Store</a>
                <a>Prank Apps</a>
                <a>Blog</a>
            </Slide>
      </div>
  </header>
</template>
<script>
import { Slide } from 'vue3-burger-menu' 
export default {
  components: {
    Slide
  }
}
</script>
<style>
    header {
        padding: 15px 20px;
        justify-content: space-between;
    }
    .nav-links-dk {
        display: none!important;
    }
    .logo-container img:first-child{
        max-width: 170px; 
    }
    .search-container {
        flex-direction: column;
        margin-left: 20px;
        background: transparent;
        border-radius: 10px;
        padding: 10px;
        max-width: 34px;
        max-height: 34px;
    }
    nav a {
        font-family: Montserrat;
        margin-left: 32px; 
        cursor: pointer;
        text-transform: uppercase;
        font-size: 13px;
    }
    .stores {
        margin-left: 32px;    
    }
    .stores div {
        border-radius: 10px;
        padding: 10px;
        border: 1px solid rgba(47, 56, 78, 0.1);
        max-width: 34px;
        max-height: 34px;
        margin-right: 10px;
    }
    .login, .sign-up {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        padding: 9px 16px;
        max-width: 73px;
        background: #2FDBD9;
        border-radius: 10px; 
        color: #fff;
        border: none;
        line-height: 16px;
        text-transform: uppercase;
        font-size: 12px;
        font-weight: 700;
    }
    .login {
        margin-right: 10px!important;
    }
    .sign-up {
        background: #FFA500;
        min-width: fit-content;
    }
    .stores div:nth-child(2) {
        margin-right: 32px;
    }
    .bm-burger-button {
        position: fixed;
        width: 20px!important;
        height: 12px!important;
        left: unset!important;
        right: 20px!important;
        top: 27px;
        cursor: pointer;
    }
    .bm-burger-bars {
      background-color: #A2A8B7;
    }
    .burger-menu img {
        margin-right: 40px;
    }
    @media(min-width:1024px) {
        .nav-links-dk {
            display: flex!important;
        }
        .burger-menu {
            display: none;    
        }
        .desktop {
            display: block;
        }
        .mobile {
            display: none;    
        }
        .search-container {
            background: rgba(47, 219, 217, 0.1);
        }
        header {
            padding: 15px 65px;
            justify-content: space-between;
        }
        .logo-container img:first-child{
            max-width: 220px; 
        }
    }
</style>
