<template>
  <div class="invoice">
    <InvoiceHeader />
    <div class="invoice__wrapper">
      <InvoiceDetails class="div1" />
      <InvoiceClient class="div2" />
      <InvoiceAmount class="div3" />
    </div>
  </div>
</template>

<script>
import InvoiceHeader from '../../components/invoices/Header.vue'
import InvoiceDetails from '../../components/invoices/Details.vue'
import InvoiceClient from '../../components/invoices/Client.vue'
import InvoiceAmount from '../../components/invoices/Amount.vue'
export default {
  components: {
    InvoiceHeader,
    InvoiceDetails,
    InvoiceClient,
    InvoiceAmount
  }
}
</script>

<style lang="scss" scoped>
.invoice__wrapper {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);
  grid-column-gap: 2rem;
  grid-row-gap: 2rem;
}

.div1 {
  grid-area: 1 / 1 / 4 / 3;
}
.div2 {
  grid-area: 1 / 3 / 2 / 4;
}
.div3 {
  grid-area: 2 / 3 / 4 / 4;
}
</style>
