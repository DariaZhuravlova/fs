<template>
  <footer class="footer">
    <div class="container">
      <a href="#header" class="logo">
        LOGO
      </a>
      <div class="contacts">
        <a href="tel:+38000000000"><atom-Phone />+380 00 000 000</a>
        <a href="mailto:aaaaaaaaaaaa@ukr.net"><atom-Email />aaaaaaaaaaaa@ukr.net</a>
      </div>
    </div>
  </footer>

</template>


<style lang="scss" scoped>
@import "@/assets/scss/main.scss";

.footer {
  background-color: $accent-dark;
  color: $bg-primary;

  .container {
    padding: 24px 32px 40px;
    display: flex;
    flex-direction: column;
  }


  .logo {
    width: 267px;
    height: 60px;
    background-color: #EEF1F4;
    border: 3px solid #545F71;
    color: black;
    display: block;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 32px;
  }

  .contacts {
    display: flex;
    flex-direction: column;
    gap: 32px;
  }

  .contacts a {
    display: flex;
    gap: 12px;
    align-items: center;
    color: #EEF1F4;
    font-size: 24px;
    font-weight: 700;
    letter-spacing: -0.02em;

  }
}

@media (min-width: 768px) {
  .footer {
    .container {
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      margin: 0;
      margin-bottom: 0;
    }
  }
}

@media (min-width: 1024px) {
  .footer .container {
    padding: 60px 72px;

    .contacts {
      flex-direction: row;
    }
  }
}

@media (min-width: 1440px) {
  .footer .container {
    .contacts {
      gap: 205px;
    }
  }
}
</style>