<script>
export default {
    name: "MainCard",
    props: {
        thumb: String,
        series: String
    }
}
</script>

<template>
    <div class="mainCard">
            <img :src="thumb" alt="comic Photo">
            <h3>{{ series }}</h3>
        </div>
    
</template>


<style scoped lang="scss">

    
    .mainCard {
        width: calc(1170px / 6 - 10px);
        margin: 20px auto;
        padding: 10px;

        img {
            width: 100%;
            height: 100%;
        }
        h3 {
            margin: 15px;
            color: white;
            font-size: .8rem;
        }
        
    }
   
</style>