<template>
  <div class="fd-margin-black"></div>
  <HeaderComponent/>
  <ContentComponent />
  <MainComponent />
  <FollowUsComponent />
  <FooterComponent />
  <div class="fd-margin-black"></div>

</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue'
  import ContentComponent from './components/ContentComponent.vue'
  import MainComponent from './components/MainComponent.vue'
  import FollowUsComponent from './components/FollowUsComponent.vue'
  import FooterComponent from './components/FooterComponent.vue'
  export default {
    name: 'App',
    components: {
      HeaderComponent,
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
  .fd-margin-black{
    height: 5vh;
    background-color: black;
  }
</style>