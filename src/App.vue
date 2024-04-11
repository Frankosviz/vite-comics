<template>
  <HeaderComponent/>
  <HeroComponent />
  <ContentComponent />
  <MainComponent />
  <FollowUsComponent />
  <FooterComponent />

</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue'
  import HeroComponent from './components/HeroComponent.vue'
  import ContentComponent from './components/ContentComponent.vue'
  import MainComponent from './components/MainComponent.vue'
  import FollowUsComponent from './components/FollowUsComponent.vue'
  import FooterComponent from './components/FooterComponent.vue'
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      HeroComponent,
      ContentComponent,
      MainComponent,
      FollowUsComponent,
      FooterComponent
    },
    data(){
      return {
        
      }
    }
  }
</script>

<style lang="scss" scoped>
</style>