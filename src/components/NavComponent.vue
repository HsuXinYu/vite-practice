<template>
  <nav class="navbar bg-light">
    <div class="container-fluid">
      <span class="navbar-brand" href="#">甜心甜點店</span>
      <div>
        購物車
        <span class="badge rounded-pill bg-danger text-white">{{ cart.length }}</span>
      </div>
    </div>
  </nav>
</template>

<script>
import cartStore from '../stores/cartStore.js'
import { mapState } from 'pinia'

export default {
  data() {
    return {}
  },
  computed: {
    ...mapState(cartStore, ['cart'])
  }
}
</script>
