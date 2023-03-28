<script>
export default {
  name: "TheHeader",
  data() {
    return {
        categoriesList: [
            "CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"
        ],
    };
  },
};
</script>

<template>
  <div class="container">
    <div class="image">
        <img src="../../src/assets/img/dc-logo.png" alt="">
    </div>

    <ul class="sectionList">
        <li v-for="(categorie, index) in categoriesList" :key="index"><a href="#">{{categorie}}</a></li>
    </ul>
  </div>
</template>

<style scooped lang="scss">

    .sectionList {
        list-style: none;
        flex-grow: 1;
        display: flex;
        justify-content: flex-end;

        li {
            padding: 10px;
            
            a {
                text-decoration: none;
                color: black;
                padding-bottom: 36px;
                

                &:hover {
                    color: rgb(53, 128, 243);
                    border-bottom: 5px solid rgb(53, 128, 243);
                }
            }

            
        }
        
    }

</style>