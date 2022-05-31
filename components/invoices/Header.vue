<template>
  <div class="invoice-header">
    <div>
      <span><span>Invoices</span> / edit invoice (INV-2022-019)</span>
    </div>
    <div class="buttons">
      <button class="btn btn--secondary">Edit</button>
      <button class="btn btn--secondary">Delete</button>
      <button class="btn btn--secondary">Mark as done</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.invoice-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 2rem 0;

  & span {
    font-size: 1.5rem;

    & span {
      color: var(--primary-color);
      font-weight: 600;
    }
  }

  .buttons {
    display: flex;
    gap: 2rem;
  }
}
</style>
