<script>
export default {
  name: "TheFooter",
  data() {
    return {
        dcComics: [
            "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"
        ],
        dcShop: [
            "Shop DC", "Shop DC Collectibles"
        ],
        dcDc: [
            "Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscription", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"
        ],
        dcSites: [
            "DC", "MAD Magazine", "DC Kids", "DC universe", "DC power Visa"
        ],
    };
  },
};
</script>

<template>
    <div class="footContainer">
        <div class="footerLists">
            <div class="firstList">
                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="(item, index) in dcComics" :key="index"><a href="#">{{ item }}</a></li>
                </ul>

                <h4>SHOP</h4>
                <ul>
                    <li v-for="(item, index) in dcShop" :key="index"><a href="#">{{ item }}</a></li>
                </ul>

            </div>
           
            <div class="firstList">
                <h4>DC</h4>
                <ul>
                    <li v-for="(item, index) in dcDc" :key="index"><a href="#">{{ item }}</a></li>
                </ul>
            </div>
           
            <div class="firstList">
                <h4>SITES</h4>
                <ul>
                    <li v-for="(item, index) in dcSites" :key="index"><a href="#">{{ item }}</a></li>
                </ul>
            </div>

            
        </div>      
    </div>
  
</template>

<style scooped lang="scss">
    .footContainer {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        height: 450px;
    }

    h4 {
        color: white;
    }

    .footerLists {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: center right;
        width: 1170px;
        margin: auto;
        display: flex;
        height: 100%;
        .firstList {
            padding: 50px;
            
            ul {
                list-style-type: none;
                padding-top: 20px;
                padding-bottom: 20px;
            }
        }
    }

    a {
        text-decoration: none;
        color: rgb(121, 121, 121);
    }
</style>