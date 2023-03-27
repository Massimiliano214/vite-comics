<script>
export default {
  name: "BottomBanner",
};
</script>

<template>
    <div class="blackBanner">
        <div class="container">
            <a class="btn" href="#">SIGN-UP NOW!</a>

            <div class="contactOptions">
                <h3>FOLLOW US</h3>
                <ul>
                    <li><a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="icona Facebook">
                    </a></li>

                    <li><a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="icona Twitter">
                    </a></li>

                    <li><a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="icona Youtube">
                    </a></li>

                    <li><a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="icona Pinterest">
                    </a></li>

                    <li><a href="#">
                        <img src="../assets/img/footer-periscope.png" alt="icona Periscope">
                    </a></li>
                </ul>
            </div>
        </div>

    </div>

  
</template>

<style scooped lang="scss">
    .blackBanner {
        background-color: rgb(51, 51, 52);

        .container {
            justify-content: space-between;

            .btn {
                border: 3px blue solid;
                padding: 10px;
                color: white;
            }
        }
    }

    .contactOptions {
        display: flex;
        align-items: center;
        color: rgb(53, 89, 168);

        ul {
            display: flex;

            li {
                list-style-type: none;
            }


            img {
                height: 50px;
                padding: 10px;
            }
        }
    }

    

</style>