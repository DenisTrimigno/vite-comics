<script>
import AppHeader from './components/AppHeader..vue';
import AppContent from './components/AppContent.vue';
import AppFooter from './components/AppFooter.vue';
import AppMenu from './components/AppMenu.vue';
import AppJumbotroon from './components/AppJumbotroon.vue';
import AppJumbo from './components/AppJumbo.vue';

export default {
  components: {
    AppHeader,
    AppContent,
    AppFooter,
    AppMenu,
    AppJumbotroon,
    AppJumbo,
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