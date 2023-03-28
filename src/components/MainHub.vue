<script>
import MainCard from './MainCard.vue';

export default {
    name: "MainHub",
    components: {
        MainCard
    },
    data() {
        return {
            comicsList: [
                {
                    "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ST_GH_Cv3_00311_DIGITAL.jpg?w=640",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640", 
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/DCConnect_35-CVR.jpg?w=640",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/LP-ROTG_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        };
    },
};
</script>


<template>
    <div class="hubBg">
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        <div class="currentSeries">
            <h3>CURRENT SERIES</h3>
        </div>
    </div>
    
    <div class="hubBottom">
        <div class="container">
            <div class="cardLayout" v-for="(comics, index) in comicsList" :key="index">
                <MainCard :thumb="comics.thumb" :series="comics.series"/>
            </div>
        </div>

        <div class="loadMore">
            <a href="#">Load More</a>
        </div>
        
    </div>
    
</template>

<style scoped lang="scss">

    .hubBg {
        position: relative;
        img {
            
            width: 100%;
            height: 400px;
            object-fit: cover;
            object-position: top;
            display: block;
            
        }
        
        .currentSeries {
            color: white;
            position: absolute;
            left: 450px;
            bottom: -15px;
            background-color: rgb(53, 128, 243);
            padding: 10px 30px;
        }
    }

    .hubBottom {
        background-color: rgb(34, 34, 34);
        padding-bottom: 30px;
        

        .container {
            flex-wrap: wrap;
            height: 100%;
            

            .cardLayout {
                
                flex-wrap: wrap;
                width: calc(100% / 6 - 10px);
                display: flex;
                flex-grow: 1;
                
                
            }
        }

        
    }

    .loadMore {
        text-align: center;
       
        
        a {
            background-color: rgb(53, 128, 243);
            color: white;
            padding: 15px 50px;
            font-size: 1.5rem;
        }
    }
</style>