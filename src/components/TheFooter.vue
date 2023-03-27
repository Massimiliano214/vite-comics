<script>
export default {
  name: "TheFooter",
};
</script>

<template>
    <div class="footContainer">
        <div class="footerLists">
            <div class="firstList">
                <h4>DC COMICS</h4>
                <ul>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                </ul>

                <h4>SHOP</h4>
                <ul>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                </ul>

            </div>
           
            <div class="firstList">
                <h4>DC</h4>
                <ul>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                </ul>
            </div>
           
            <div class="firstList">
                <h4>SITES</h4>
                <ul>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
                    <li><a href="#">lorem</a></li>
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
        color: darkgrey;
    }
</style>