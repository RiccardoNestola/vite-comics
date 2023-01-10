<script>

export default {

    /* components: {
        ProductComp,
  }, */

    props:{
        imgPath: String,
        price: Number,
        series: String,
        type:String
    },
    
    
}
</script>

<template>
    <div class="book_element">
        <div class="wrapper">
            <img :src="imgPath" :alt="type">   
        </div>
        
        <p>{{ series }}</p>
    </div>
</template>

<style lang="scss" scoped>

.book_element{
            width: calc(100% / 6 - 1rem);
            margin:.5rem;
            height: 200px;

            img{
                width: 100%;
                height: auto;

            }
            p{
                text-transform: uppercase;
                font-size: .6rem;
            }
        }
    
</style>