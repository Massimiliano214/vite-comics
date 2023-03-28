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
        width: calc(1170px / 6 - 40px);
        margin: 20px auto;
        display: flex;
        flex-direction: column;

        img {
            width: 100%;
            height: 100%;
            align-self: flex-start;
        }
        
    }
    h3 {
            margin: 15px;
            color: white;
        }
</style>