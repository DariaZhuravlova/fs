<template>
  <section class="about" id="about">
    <div class="container">
      <img src="@/assets/images/about.png" alt="about image">
      <div>
        <h2>Що таке особиста веб-сторінка і <br>
          кому вона потрібна?</h2>
        <p><strong>Особиста веб-сторінка</strong> – це односторінковий сайт з привабливим дизайном і продуманою
          структурою. Вона призначена
          для просування одного товару або послуги.

        </p>
        <p>Основна мета такого сайту – залучити якомога більше потенційних клієнтів.</p>
        <p>Особиста веб-сторінка стане в нагоді всім, хто зацікавлений у швидких продажах конкретного товару або
          просуванні послуг.</p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/main.scss';

.about {
  background-color: $bg-secondary;

  .container {
    padding: 16px;
  }

  img {
    width: 277px;
    height: 169px;
    display: block;
    margin: 0 auto;
    margin-bottom: 24px;
  }

  h2 {
    margin-bottom: 24px;
  }

  strong {
    font-size: 20px;
    font-weight: 700;
    letter-spacing: -0.02em;
  }

  p:not(:last-child) {
    margin-bottom: 26px;
  }
}

@media (min-width: 768px) {
  .about {
    .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 24px;
    }

    img {
      width: calc((100% - 24px)/2);
      margin-bottom: 0;
      max-width: 636px;
      height: auto;
    }
  }
}

@media (min-width: 1024px) {
  .about {
    .container {
      padding: 60px 72px;
    }
  }
}
</style>