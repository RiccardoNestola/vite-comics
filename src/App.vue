<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';
import BannerComp from './components/BannerComp.vue';

export default {
  
  components: {
	HeaderComp,
  MainComp,
  FooterComp,
  BannerComp
  }

}

</script>

<template>

<HeaderComp/>

<BannerComp/>

<MainComp/>

<FooterComp/>
  
  
</template>

<style lang="scss">
    @use "./styles/general" as *;
    @use "./styles/partials/variables" as *;         

</style>
