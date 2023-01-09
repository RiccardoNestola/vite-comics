<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';


export default {
  
  components: {
	HeaderComp,
  MainComp,
  FooterComp
  }

}

</script>

<template>

<HeaderComp/>

<MainComp/>

<FooterComp/>
  
  
</template>

<style lang="scss">
    @use "./styles/general" as *;
    @use "./styles/partials/variables" as *;         

</style>
