<script>

export default {
  
  components: {
	
  }

}

</script>

<template>

  <main>
    <h2>Content goes here</h2>
  </main>
  
</template>

<style lang="scss" scoped>
    @use "../styles/general.scss" as *;
    @use "../styles/partials/variables" as *;     
    
        main{
          background-color: black;
          color: white;
          width: 100%;

          h2{
            padding: 3rem;
          }
        }

</style>