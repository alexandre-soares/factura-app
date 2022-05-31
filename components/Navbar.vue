<template>
  <div class="navbar">
    <div class="navbar__left">
      <div class="navbar__brand">
        <span>Factura App.</span>
      </div>
      <ul class="navbar__list">
        <li class="navbar__item"><a href="#">Dashboard</a></li>
        <li class="navbar__item">Invoices</li>
      </ul>
    </div>
    <div class="navbar__right"></div>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style lang="scss" scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 3rem 0;

  &__left {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 5rem;
  }

  &__list {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 4rem;
    list-style-type: none;
    padding: 0;
  }

  &__item {
    font-size: 1.7rem;
    margin-bottom: -1px;
    font-weight: 500;
  }

  & span {
    color: var(--primary-color);
    font-weight: 600;
    font-size: 1.9rem;
  }
}
</style>
