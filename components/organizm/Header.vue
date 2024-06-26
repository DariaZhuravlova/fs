<template>
  <header class="header">
    <div class="container">
      <div class="menu">
        <a href="/" class="logo">LOGO</a>
      <button class="menu-toggle" @click="toggleMenu">
        <span></span>
        <span></span>
        <span></span>
      </button>
      </div>
      <nav :class="{ 'nav-links': true, 'open': menuOpen }">
        <a href="#about" @click="closeMenu">Про веб-сторінку</a>
        <a href="#offer" @click="closeMenu">Пропозиції та ціни</a>
        <a href="#steps" @click="closeMenu">Кроки розробки</a>
      </nav>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const menuOpen = ref(false);

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};

const closeMenu = () => {
  menuOpen.value = false;
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/main.scss";
.header {
  .container {
    padding: 16px;
    // display: flex;
    // justify-content: space-between;
    // align-items: center;
    position: relative;
    // flex-direction: column;
    @media (min-width: 1024px) {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      gap: 40px;
      padding: 60px 72px 40px;
    }

    .menu {
      // width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    
  }

  .logo {
    display: block;
    padding: 8px 16px;
    width: 166px;
    height: 60px;
    background-color: #eef1f4;
    border: 3px solid #545f71;
    color: black;
    text-align: center;
    text-decoration: none;
    @media (min-width: 1024px){
      width: 307px;
    }
  }

  .menu-toggle {
    display: flex;
    flex-direction: column;
    gap: 4px;
    background: none;
    border: none;
    cursor: pointer;

    span {
      display: block;
      width: 50px;
      height: 4px;
      background: $accent-light;
    }
  }

  .nav-links {
    display: none;
    flex-direction: column;
    width: 100%;
    max-width: 675px;
    // background-color: #eef1f4;
    padding: 16px;
    gap: 12px;

    a {
      color: #282828;
      text-decoration: none;
      font-size: 18px;
      font-weight: 400;
      line-height: 1.6;
    }

    a:hover {
      color: $accent-dark;
    }

    a:active {
      color: $accent-dark;
      text-decoration: underline;
    }

    &.open {
      display: flex;
      flex-direction: column;
    }
  }

  .menu-open .nav-links {
    display: flex;
    flex-direction: column;
    width: 100%;
    background-color: #eef1f4;
    padding: 16px;
    gap: 12px;
  }

  @media (min-width: 1024px) {
    
    .nav-links {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      background-color: transparent;
      padding: 0;
      // width: auto;

      a {
        margin-bottom: 0;
        margin-right: 24px;
      }

      a:last-child {
        margin-right: 0;
      }
    }

    .menu-toggle {
      display: none;
    }

    .menu-open .nav-links {
      display: flex;
      flex-direction: row;
    }
  }
}
</style>






