<template>
  <section class="amount">
    <h4>Amount Due <span class="text-grey">(USD)</span></h4>
    <span class="price"
      >$4,800.00 <span class="text-grey">(Tax Incl.)</span></span
    >
    <span class="due-date">Due on Jan 20, 2022</span>
    <hr />
    <div class="flex attach">
      <span>Also attach pdf in mail</span>
      <input type="radio" name="yes" />
    </div>
    <div class="flex">
      <button class="btn btn--secondary">Preview</button>
      <button class="btn btn--secondary">Download</button>
    </div>
    <button class="btn btn--primary block">Send Invoice</button>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.block {
  display: block;
  width: 100%;
}

.btn--primary {
  padding: 2rem;
}

.price {
  font-size: 2.5rem;
  font-weight: 800;
  margin: 2rem 0 1rem;
  display: block;

  & span {
    font-size: 1.8rem;
    font-weight: 400;
  }
}

.due-date {
  display: inline-block;
  padding: 1rem 2rem;
  background-color: #fdeeef;
  color: #f1666a;
  font-size: 1.4rem;
  font-weight: 600;
  margin: 2rem 0 1rem;
  border-radius: 2rem;
}

hr {
  margin: 2rem 0;
}

.attach {
    font-size: 1.5rem;
    font-weight: 600;
}
</style>
