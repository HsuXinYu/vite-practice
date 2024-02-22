<script>
// import { RouterLink, RouterView } from 'vue-router'
import NavComponent from './components/NavComponent.vue'
import CartComponent from './components/CartComponent.vue'
import ProductComponent from './components/ProductComponent.vue'

export default {
  components: {
    NavComponent,
    CartComponent,
    ProductComponent
  }
}
</script>

<template>
  <div class="container">
    <NavComponent></NavComponent>
    <CartComponent></CartComponent>
    <ProductComponent></ProductComponent>
  </div>
</template>

<style lang="scss">
@import 'assets/all.scss';
</style>
