<script>
import AppHeader from './components/AppHeader.vue'
import ListProducts from './components/ListProducts.vue'
import NavList from './components/NavList.vue'
import AppFooter from './components/AppFooter.vue'

export default{
  components:{
    AppHeader,
    ListProducts,
    NavList,
    AppFooter
  }
}
</script>

<template>
  <header>
    <AppHeader/>
  </header>

  <main>
    <ListProducts/>
    <NavList/>
  </main>

  <footer>
    <AppFooter/>
  </footer>
</template>

<style lang="scss">
  @use './styles/partials/variables' as *;
  @use './styles/general.scss' as *;
</style>
