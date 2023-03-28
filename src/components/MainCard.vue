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
    <div class="allCard">
        <div class="mainCard">
            <img :src="thumb" alt="comic Photo">
        </div>

        <h3>{{ series }}</h3>
    </div>
    
</template>


<style scoped lang="scss">

    .allCard {
        height: 100%;
    }
    .mainCard {
        width: calc(1170px / 6 - 40px);
        margin: 20px;

        img {
            width: 100%;
            height: 100%;
        }
        
    }
    h3 {
            margin: 15px;
            color: white;
        }
</style>