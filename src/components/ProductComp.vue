<script>

export default {

    props:{
        img: String,
        price: Number,
        series: String,
        type:String
    }
    
}
</script>

<template>
    <div>
        <img :src="img" :alt="type">
        <h2>{{ series }}</h2>
    </div>
</template>

<style lang="scss" scoped>
    
</style>