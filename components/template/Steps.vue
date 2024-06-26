<template>
  <section class="steps" id="steps">
    <div class="container">
      <h2 class="title">Ми пропонуємо нашим клієнтам</h2>
      <div class="step-cards">
        <div class="step-1">
          <div class="step-info">
            <div class="step-title">
              <span>01</span>
              <h2>Аналіз конкурентів</h2>
            </div>
            <p class="step-description">Важливий етап у процесі розробки кожної веб-сторінки. Він включає дослідження
              ринку,
              виявлення конкурентних
              переваг і недоліків продукту. Детальний аналіз конкурентів допомагає створити унікальну торгову пропозицію
              для
              продукту та уникнути помилок у його подальшому просуванні.</p>
          </div>
          <img src="@/assets/images/step-1.jpg" alt="step 1">
        </div>
        <div class="step-2">
          <div class="step-info">
            <div class="step-title">
              <span>02</span>
              <h2>Створення дизайну</h2>
            </div>
            <p class="step-description">Розробка дизайну є важливою частиною процесу створення сайту, оскільки вона
              визначає
              вигляд та користувацький
              інтерфейс сайту.
              Розробка дизайну - це творчий процес, і важливо враховувати бажання та потреби замовника, а також
              забезпечувати
              кращий користувацький досвід для відвідувачів сайту.</p>
          </div>
          <img src="@/assets/images/step-2.jpg" alt="step 2">
        </div>
        <div class="step-1">
          <div class="step-info">
            <div class="step-title">
              <span>03</span>
              <h2>Створення веб-сторінки</h2>
            </div>
            <p class="step-description">Розробка веб-сторінки охоплює створення та запуск веб-простору для вашого
              бізнесу чи проєкту. Від збору вимог і проєктування до програмування й тестування, цей процес допомагає
              втілити вашу ідею в життя та забезпечити присутність в Інтернеті для досягнення ваших бізнес-цілей.</p>
          </div>
          <img src="@/assets/images/step-3.jpg" alt="step 3">
        </div>
        <div class="step-4">
          <div class="step-info">
            <div class="step-title">
              <span>04</span>
              <h2>Тестування</h2>
            </div>
            <p class="step-description">Завершальний етап у процесі створення веб-сторінки включає перевірку сайту на
              наявність помилок у програмному коді та коректність відображення на різних мобільних гаджетах. Також
              проводиться тестування роботи сайту в різних операційних системах.</p>
          </div>
          <img src="@/assets/images/step-4.jpg" alt="step 4">
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/main.scss';

.steps {
  background-color: $bg-secondary;

  .container {
    padding: 16px;
  }

  .title {
    text-align: center;
  }

  .step-title {
    display: flex;
    gap: 12px;
    align-items: center;
  }

  span {
    font-size: 96px;
    font-weight: 700;
    line-height: 134.4px;
    letter-spacing: -0.02em;
    text-align: left;
    color: transparent;
    font-family: 'Saira', sans-serif;
    -webkit-text-stroke: 3px $accent-dark;
  }

  .step-description {
    margin-bottom: 12px;
    line-height: 1.6;
  }

  img {
    width: 100%;
    max-width: 400px;
    height: auto;
  }
}

@media (min-width: 768px) {
  .steps {
    .step-cards {
      display: flex;
      flex-direction: column;
      gap: 24px;
    }

    .step-title {
      gap: 24px;
      margin-bottom: 24px;
    }

    img {
      width: calc((100% - 24px)/2);
      height: auto;
      max-width: none;
    }
  }

  .step-1,
  .step-2,
  .step-3,
  .step-4 {
    display: flex;
    justify-content: space-between;
    gap: 24px;
  }

  .step-1,
  .step-3 {
    flex-direction: row-reverse;
  }
  }


@media (min-width: 1024px) {
  .steps {
    .container {
      padding: 60px 72px;
    }

    .title {
      margin-bottom: 40px;
    }
  }
}
</style>