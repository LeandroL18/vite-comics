<script>
import AppHeader from './components/AppHeader.vue'
import ListProducts from './components/ListProducts.vue'

export default{
  components:{
    AppHeader,
    ListProducts
  }
}
</script>

<template>
  <header>
    <AppHeader/>
  </header>

  <main>
    <ListProducts/>
  </main>

  <footer>

  </footer>
</template>

<style lang="scss">
  @use './styles/partials/variables' as *;
  @use './styles/general.scss' as *;
</style>
