<script>
    export default {
        name: "MainBanner",
    };
</script>

<template>
    <div class="mainBanner">
        <div class="containerBannerMain">
            <ul>
                <li><img src="../assets/img/buy-comics-digital-comics.png" alt="">DIGITAL COMICS</li>
                <li><img src="../assets/img/buy-comics-merchandise.png" alt="">DC MERCHANDISE</li>
                <li><img src="../assets/img/buy-comics-subscriptions.png" alt="">SUBSCRIPTION</li>
                <li><img src="../assets/img/buy-comics-shop-locator.png" alt="">COMIC SHOP LOCATOR</li>
                <li><img src="../assets/img/buy-dc-power-visa.svg" alt="">DC POWER VISA</li>
            </ul>
        </div>
        
    </div>
</template>

<style scoped lang="scss">
    .mainBanner {
        background-color: rgb(53, 128, 243);

        .containerBannerMain {
            widows: 1170px;
            justify-content: center;
            display: flex;
            padding: 30px;
            
            ul {
                display: flex;
                list-style-type: none;
                align-items: center;

                li {
                    display: flex;
                    align-items: center;
                    color: white;
                    padding-left: 20px;
                    padding-right: 20px;
                }

                img {
                    height: 50px;
                    margin: 10px;
                }
            }
        }
    }
</style>