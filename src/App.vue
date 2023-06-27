<script>
import AppHeader from './components/AppHeader..vue';
import AppContent from './components/AppContent.vue';
import AppFooter from './components/AppFooter.vue';
import AppMenu from './components/AppMenu.vue';

export default {
  components: {
    AppHeader,
    AppContent,
    AppFooter,
    AppMenu,
  }
  
}
</script>

<template lang="">
  <div>

    <AppHeader/>
    <AppContent/>
    <AppFooter/>
    <AppMenu/>

  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
  
</style>