<script>
import AppHeader from './components/AppHeader..vue';
import AppContent from './components/AppContent.vue';
import AppFooter from './components/AppFooter.vue';
import AppMenu from './components/AppMenu.vue';
import AppJumbotroon from './components/AppJumbotroon.vue';

export default {
  components: {
    AppHeader,
    AppContent,
    AppFooter,
    AppMenu,
    AppJumbotroon
  }
  
}
</script>

<template lang="">
  <div>

    <AppHeader/>
    <AppContent/>
    <AppMenu/>
    <AppJumbotroon/>
    <AppFooter/>
    
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
  
</style>