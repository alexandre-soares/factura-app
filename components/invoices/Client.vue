<template>
  <section class="client">
    <h4>Client Details</h4>
    <div class="client__name">
      <div class="logo"></div>
      <div class="fullname">
        <h3>Zaky Grizzly</h3>
        <p>grizzly@moonlight.com</p>
      </div>
    </div>
    <div class="client__address">
      <h5>Monlight Agenct LTD</h5>
      <p>9 Acacia Drive Rome, NY 13440, USA</p>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.client {
  &__name {
    margin: 2rem 0;
  }

  h3,
  h5 {
    font-size: 1.6rem;
    margin-bottom: 1rem;
  }

  p {
    color: var(--text-grey);
    font-size: 1.4rem;
  }
}
</style>
