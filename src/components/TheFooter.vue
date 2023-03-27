<script>
export default {
  name: "TheFooter",
  data() {
    return {
        dcComics: [
            "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"
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
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>

            </div>
           
            <div class="firstList">
                <h4>DC</h4>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscription</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
           
            <div class="firstList">
                <h4>SITES</h4>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC universe</a></li>
                    <li><a href="#">DC power Visa</a></li>
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