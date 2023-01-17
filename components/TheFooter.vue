<template>
  <footer id="footer" class="footer">
    <div class="footer__container">
      <nav class="footer__nav">
        <NuxtLink class="footer__link" to="/">Главная</NuxtLink>
        <NuxtLink class="footer__link" to="/">О нас</NuxtLink>
        <NuxtLink class="footer__link" to="/">Каталог</NuxtLink>
        <NuxtLink class="footer__link footer__link_gray" to="/">Доставка</NuxtLink>
        <NuxtLink class="footer__link" to="/">Помощь</NuxtLink>
      </nav>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background-color: var(--black);

  &__container {
    display: flex;
    align-items: center;
    margin: 0 auto;
    width: 1200px;
    height: 100px;
  }

  &__nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }

  &__link {
    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
    color: var(--white);

    &_gray {
      color: var(--gray);
    }
  }
}
</style>
