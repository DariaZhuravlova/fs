<template>
<section class="hero container" id="hero">
  <img src="@/assets/images/hero.png" alt="hero image" class="hero-img">
  <div>
    <h1>Створення Landing Page під ключ</h1>
    <p>Ми спеціалізуємося на створенні ефективних Landing Page з унікальним UX-дизайном. Наші лендінги не лише продають, але й збільшують кількість клієнтів та підвищують ваш прибуток!</p>
    <div class="contacts">
      <a href="tel:+38000000000">
        <atom-Phone />+380 00 000 000</a>
      <a href="mailto:aaaaaaaaaaaa@ukr.net">
        <atom-Email />aaaaaaaaaaaa@ukr.net</a>
    </div>
  </div>
  
</section>
</template>


<style lang="scss" scoped>
@import '@/assets/scss/main.scss';

  .hero {
    padding: 16px;
  }

  .hero-img {
    width: 100%;
    max-width: 274px;
    height: 180px;
    display: block;
    margin: 0 auto;
    margin-bottom: 12px;
  }

  .hero h1, .hero p {
    margin-bottom: 12px;
  }

  .hero .contacts {
    display: flex;
    flex-direction: column;
    gap: 24px;
  }

  .hero .contacts a {
    display: flex;
    align-items: center;
    gap: 8px;
    font-weight: 700;
    font-size: 20px;
    line-height: 28px;
    color: $primary-medium;
   
  }

  
  @media (min-width: 768px) {
    .hero {
      display: flex;
      flex-direction: row-reverse;
      align-items: center;
      justify-content: space-between;

      .hero-img {
        width: calc((100% - 24px)/2);
        margin-bottom: 0;
        max-width: 636px;
        height: auto;
      }
    }
  }

  @media (min-width: 1024px) {
    .hero {
      padding: 60px 72px;
      
    }
  }

  @media (min-width: 1440px) {
    .hero  {
      padding: 145px 72px;
      h1, p {
        margin-bottom: 74px;
      }

      .contacts {
        flex-direction: row;
        gap: 72px;
      }
    }
  }
</style>