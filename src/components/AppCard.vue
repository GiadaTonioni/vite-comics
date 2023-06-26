<script>
export default {
    props: {
        img: String,
        series: String,
        price: String,
        type: String,
    }
}
</script>

<template lang="">
    <div class="card">
        <img :src="image">
        <h5>{{series}}</h5>
        <p>{{type}}</p>
        <p>{{price}}</p>
    </div>
</template>

<style lang="">
    
</style>