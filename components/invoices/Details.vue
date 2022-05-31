<template>
  <section class="details">
    <div class="from">
      <div class="from__name-infos">
        <div class="logo"></div>
        <div class="name">
          <h1>Dipa Inhouse</h1>
          <h2>hello@dipainhouse.com</h2>
        </div>
      </div>
      <div class="from__address">
        <p>Ijen Boulevard Street 101</p>
        <p>Malang City, 65115</p>
        <p>East Java, Indonesia</p>
      </div>
    </div>
    <div class="basic-infos">
      <div class="invoice-number">
        <h3>Invoice Number</h3>
        <p>INV-2022-010</p>
        <p>Issued Date: 11 Jan 2022</p>
        <p>Due Date: 18 Jan 2022</p>
      </div>
      <div class="billed-to">
        <h3>Billed to</h3>
        <p>Zaky grizzly</p>
        <p>Monlight Agency LTD</p>
        <p>New York, USA</p>
      </div>
    </div>
    <div class="items-details">
      <h4>Item Detail</h4>
      <table class="item-list">
        <tr class="table-heading">
          <th class="item-name">Item Name</th>
          <th class="rate">Rate/hr</th>
          <th class="tax">Tax</th>
          <th class="total">Line Total</th>
        </tr>
      </table>
      <hr />
      <div class="payment-method">
        <div class="account">
          <h4>Payment Method</h4>
          <h5>Wire Transfer</h5>
          <p>Account Name: <span>Barley Vallendito</span></p>
          <p>Routing Numner: <span>0000 1111 2222 3333</span></p>
          <p>Account Number: <span>Barley Vallendito</span></p>
        </div>
        <div class="resume">
          <div class="subtotal flex">
            <p>Sub Total</p>
            <p class="black">$4,8000.00</p>
          </div>
          <div class="discount flex">
            <p>Discount</p>
            <p class="black">$0.00</p>
          </div>
          <div class="total-tax flex">
            <p>Total tax</p>
            <p class="black">$0.00</p>
          </div>
          <hr />
          <div class="total-amount flex">
            <p>Total Amount</p>
            <p class="black">$4,800.00</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Details'
}
</script>

<style lang="scss" scoped>
.flex {
  display: flex;
  justify-content: space-between;
}
.details {
  border-radius: 1rem;
}

.from {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;

  &__name-infos {
    & h1 {
      font-size: 1.8rem;
      margin-bottom: 1rem;
    }

    & h2 {
      color: var(--text-grey);
    }
  }

  &__address {
    font-size: 1.4rem;
    color: var(--text-grey);
    line-height: 1.6;
    text-align: right;
  }
}

.basic-infos {
  background-color: var(--primary-color);
  padding: 2rem 3rem;
  border-radius: 1rem;
  margin: 2rem 0;
  color: white;
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 1.4rem;
  font-weight: 400;
  line-height: 1.9;

  & h3 {
    font-size: 1.4rem;
    font-weight: 600;
    letter-spacing: 0.4px;
  }
  & p {
    font-size: 1.4rem;
    font-weight: 300;
  }

  .billed-to {
    text-align: right;
  }
}

.items-details {
  padding: 2rem 0;
}
.items-details {
  table tr {
    display: flex;
    align-items: center;
    margin: 3rem 0;
  }

  .item-list {
    width: 100%;
  }

  .table-heading,
  .table-items {
    gap: 16px;
    font-size: 1.4rem;
    color: var(--text-grey);

    .item-name {
      flex-basis: 50%;
      font-weight: 500;
    }
    .rate {
      flex-basis: 10%;
      font-weight: 500;
    }
    .tax {
      flex-basis: 20%;
      font-weight: 500;
    }
    .total {
      flex-basis: 20%;
      font-weight: 500;
      align-self: center;
    }
  }
  .table-heading {
    th {
      text-align: left;
    }
  }
  .table-items {
    position: relative;
    margin-bottom: 24px;
    img {
      position: absolute;
      top: 15px;
      right: 0;
      width: 12px;
      height: 16px;
    }
  }

  .payment-method {
    margin: 3rem 0;
    display: flex;
    align-items: flex-start;
    justify-content: space-between;

    & h5 {
      margin: 2rem 0 1rem;
      font-size: 1.4rem;
    }

    & p {
      font-size: 1.3rem;
      color: var(--text-grey);
      line-height: 1.8;
      & > span {
        color: var(--text-black);
        font-weight: bold;
      }
    }

    .resume {
      display: flex;
      gap: 2rem;
      flex-direction: column;
      justify-content: space-between;

      & div {
        gap: 10rem;
      }
    }
  }
}
</style>
