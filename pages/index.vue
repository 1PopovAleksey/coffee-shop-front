<template>
  <div>
    <section id="hero" class="hero">
      <div class="hero__container">
        <div class="hero__flex">
          <h1 class="hero__title">
            <span class="hero__title_gray">КОФЕ</span>
            С ДОСТАВКОЙ ПО ВСЕМУ МИРУ
          </h1>
          <button class="hero__btn">В каталог</button>
        </div>
        <img class="hero__img" src="~/assets/img/hero.png" alt="Фотография нашей кофейни" />
      </div>
    </section>
    <section id="about-us" class="about-us">
      <div class="about-us__container">
        <img class="about-us__img" src="~/assets/img/about-us-1.png" alt="" />
        <div class="about-us__flex">
          <div class="about-us__content">
            <p class="about-us__company">Компания</p>
            <h2 class="about-us__title">CoffeeShop</h2>
            <p class="about-us__text">
              Задача организации, в особенности же постоянное информационно пропагандистское
              обеспечение нашей деятельности обеспечивает широкому кругу
            </p>
          </div>
        </div>
        <img class="about-us__img" src="~/assets/img/about-us-2.png" alt="" />
      </div>
    </section>
    <section id="why-we" class="why-we">
      <div class="why-we__container">
        <div class="why-we__offset">
          <h2 class="why-we__title">ПОЧЕМУ БОЛЕЕ 5.000 ЧЕЛОВЕК ВЫБРАЛИ НАС?</h2>
          <div class="why-we__flex">
            <ul class="why-we__list why-we__list_left">
              <li class="why-we__item">
                <h3 class="why-we__item-title">Качество</h3>
                <p class="why-we__item-description" style="text-align: end">Самые свежие зерна</p>
              </li>
              <li class="why-we__item">
                <h3 class="why-we__item-title">Вкус</h3>
                <p class="why-we__item-description" style="text-align: end">
                  Превосходный кофе на любой вкус
                </p>
              </li>
              <li class="why-we__item">
                <h3 class="why-we__item-title">Инновации</h3>
                <p class="why-we__item-description" style="text-align: end">
                  Кофемашины последних моделей
                </p>
              </li>
            </ul>
            <img class="why-we__img" src="~/assets/img/why-we.png" alt="Почему мы?" />
            <ul class="why-we__list why-we__list_right">
              <li class="why-we__item">
                <h3 class="why-we__item-title">Выгода</h3>
                <p class="why-we__item-description">Лучшие цены</p>
              </li>
              <li class="why-we__item">
                <h3 class="why-we__item-title">Скорость</h3>
                <p class="why-we__item-description">Быстрая доставка и обслуживание</p>
              </li>
              <li class="why-we__item">
                <h3 class="why-we__item-title">Экологичность</h3>
                <p class="why-we__item-description">Экологичное производство</p>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
};
</script>

<style lang="scss" scoped>
@import '../assets/scss/mixins.scss';

.hero {
  &__container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    @include container;
    height: 600px;
  }

  &__flex {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 30px;
    width: 609px;
  }

  &__title {
    font-weight: 600;
    font-size: 54px;
    line-height: 66px;
    color: var(--black);

    &_gray {
      color: var(--gray);
    }
  }

  &__btn {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 250px;
    height: 60px;
    border: none;
    border-radius: 10px;
    font-weight: 500;
    font-size: 24px;
    line-height: 29px;
    color: var(--black);
    background: var(--gray);
  }

  &__img {
    width: 450px;
    height: 450px;
    border-radius: 60px;
  }
}

.about-us {
  &__container {
    display: flex;
    width: 100%;
  }

  &__img {
    width: 450px;
    height: 450px;
  }

  &__flex {
    display: flex;
    flex-direction: column;
    padding: 50px;
    width: 100%;
    height: 450px;
    background-color: var(--black);
  }

  &__content {
    max-width: 440px;
  }

  &__company {
    font-weight: 400;
    font-size: 36px;
    line-height: 44px;
    letter-spacing: 0.01em;
    color: var(--white);
  }

  &__title {
    margin: 5px 0 0 0;
    font-weight: 600;
    font-size: 36px;
    line-height: 44px;
    letter-spacing: 0.05em;
    color: var(--white);
  }

  &__text {
    margin: 40px 0 0 0;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    color: var(--white);
  }
}

.why-we {
  &__container {
    @include container;
  }

  &__offset {
    padding: 90px 0;
  }

  &__title {
    width: 682px;
    font-weight: 600;
    font-size: 48px;
    line-height: 59px;
    color: var(--black);
  }

  &__flex {
    display: flex;
    padding: 0 27px;
    margin: 70px 0 0 0;
  }

  &__list {
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    &_left {
      li {
        display: flex;
        flex-direction: column;
        align-items: flex-end;
      }
    }

    &_right {
      li {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
      }
    }
  }

  &__item {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  &__item-title {
    font-weight: 600;
    font-size: 32px;
    line-height: 39px;
    color: var(--black);
  }

  &__item-description {
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    color: var(--black);
  }

  &__img {
    padding: 0 107px;
  }
}
</style>
