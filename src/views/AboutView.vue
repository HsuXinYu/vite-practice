<script>
export default {
  data() {
    return {
      user: {}
    }
  },
  mounted() {
    this.axios.get('https://randomuser.me/api/').then((response) => {
      // console.log(response.data)
      this.user = response.data.results[0]
      console.log(this.user)
    })
    // or
    // this.$http.get(api).then((response) => {
    //   console.log(response.data)
    // })
  }
}
</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
    {{ this.user.name.first }}
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
