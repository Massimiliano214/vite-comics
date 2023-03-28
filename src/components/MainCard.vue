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

</style>