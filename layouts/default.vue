<template>
  <div class="container">
    <Navbar />
    <Nuxt />
  </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'
export default {
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
:root {
  --primary-color: #4e4ea6;
  --secondary-color: #3634c5;
  --text-black: black;
  --text-grey: #646464;
  --primary-white: #ffffff;
  --primary-background-color: #efefef;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  font-size: 62.5%;
  font-family: 'Poppins', sans-serif;
  background-color: var(--primary-background-color);
}

.container {
  max-width: 1440px !important;
  padding-right: 10rem !important;
  padding-left: 10rem !important;
  margin: 0 auto;
}
@media only screen and (max-width: 1200px) {
  .container {
    padding: 1.2rem 4.8rem !important;
  }
}
@media only screen and (max-width: 768px) {
  .container {
    padding: 1.2rem 2.4rem !important;
  }
}
@media only screen and (max-width: 479px) {
  .container {
    padding: 1.2rem 1.6rem !important;
  }
}

a {
  text-decoration: none;
}

section {
  background-color: var(--primary-white);
  padding: 2rem 3rem;
  border-radius: 1rem;
}

.btn {
  padding: 1rem 2rem;
  border-radius: 1rem;
  border: none;
  font-size: 1.6rem;
  font-weight: 900;
  cursor: pointer;

  &--primary {
    background-color: var(--primary-color);
    color: var(--primary-white);
  }

  &--secondary {
    background-color: var(--primary-white);
    color: var(--primary-color);
  }
}

p.black {
  color: var(--text-black) !important;
  font-weight: bolder;
}

h4 {
  font-size: 1.6rem;
  margin-bottom: 1rem;
}

</style>
