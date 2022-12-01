<template>
  <div>
    <img src="../assets/spotify-logo-png-7053.png" alt="">
    <SearchComp />
  </div>
</template>

<script>
import SearchComp from './components/SearchComp.vue'

export default {
  name: 'HeaderComp',
  components: {
    SearchComp
  },
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

img {
  width: 50px;
}
</style>
