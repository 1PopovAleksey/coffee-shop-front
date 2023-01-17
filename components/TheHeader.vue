<template>
  <header id="header" class="header">
    <div class="header__container">
      <nav class="header__nav">
        <NuxtLink class="header__link" to="/">Главная</NuxtLink>
        <NuxtLink class="header__link" to="/">О нас</NuxtLink>
        <NuxtLink class="header__link" to="/">Каталог</NuxtLink>
        <NuxtLink class="header__link header__link_gray" to="/">Доставка</NuxtLink>
        <NuxtLink class="header__link" to="/">Помощь</NuxtLink>
      </nav>
      <a class="header__link" href="tel:+79999999999">+7 (999) 999 99 99</a>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  box-shadow: 0px 0px 20px rgba(11, 10, 10, 0.1);

  &__container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;
    width: 1200px;
    height: 100px;
  }

  &__nav {
    display: flex;
    align-items: center;
    gap: 30px;
  }

  &__link {
    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
    color: var(--black);

    &_gray {
      color: var(--gray);
    }
  }
}
</style>
