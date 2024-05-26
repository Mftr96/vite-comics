<script>
export default {
  data() {
    return {
        photos:[
            {percorso:"../../src/assets/img/buy-comics-digital-comics.png",
                txt:"DIGITAL COMICS"
            },
            {percorso:"../../src/assets/img/buy-comics-merchandise.png",
                txt:"MERCHANDISE"
            },
            {percorso:"../../src/assets/img/buy-comics-subscription.png",
                txt:"SUBSCRIPTION"
            },
            {percorso:"../../src/assets/img/buy-comics-shop-locator.png",
                txt:"COMIC SHOP LOCATOR"
            },
            {percorso:"../../src/assets/img/buy-dc-power-visa.svg",   
                txt:"DC POWER VISA"
            }
        ],
         fumetti: [
    {
        thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
        price: "$19.99",
        series: "Action Comics",
        type: "comic book",
    },
    {
        thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
        price: "$3.99",
        series: "American Vampire 1976",
        type: "comic book",
    },
    {
        thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
        price: "$16.99",
        series: "Aquaman",
        type: "graphic novel",
    },
    {
        thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
        price: "$2.99",
        series: "Batgirl",
        type: "comic book",
    },
    {
        thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
        price: "$3.99",
        series: "Batman",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
        price: "$2.99",
        series: "Batman Beyond",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
        price: "$3.99",
        series: "Batman/Superman",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
        price: "$4.99",
        series: "Batman/Superman Annual",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
        price: "$5.99",
        series: "Batman: The Joker War Zone",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
        price: "$6.99",
        series: "Batman: Three Jokers",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
        price: "$4.99",
        series: "Batman: White Knight Presents: Harley Quinn",
        type: "comic book",
    },
    {
        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
        price: "$16.99",
        series: "Catwoman",
        type: "graphic novel",
    },
]

    }
  },
  methods: {
    //funzioni Vue 
  },
  mounted() {
    console.log("App montata Main");
  }
}

</script>
<template>
    <main>
        <section class="main-upper">
            <div class="container-upper">
                <div v-for="comic in fumetti" class="card-upper">
                    <img :src="comic.thumb" alt="">
                    <p>{{comic.series.toUpperCase() }}</p>
                </div>
            </div>
        </section>

        <section class="main-lower">
            <div class="container-lower">
                <div v-for="image in photos" class="card-lower">
                    <img :src="image.percorso" alt=""> 
                    <p>{{image.txt}}</p>
                </div>    
            </div>
        </section>
    </main>

</template>

<style scoped>
    .container-upper{
        width: 1300px;
        display: flex;
        flex-wrap: wrap;
        gap: 1rem;
        margin: 0 auto;
    }

    .main-upper{
        background-color: rgb(28, 28, 28);
        color: white;
        padding: 6rem;
    }
    .card-upper{
        width:200px;
        height:200px;
        margin-bottom: 2rem;
    }
    .main-upper>.container-upper img{
        width: 100%;
        height: 100%;
    }
    .main-upper>.container-upper p{
        width:100%;
    }
    /* --------MAIN-LOWER STYLE------------------------------ */
    .container-lower{
        width: 1300px;
        display: flex;
        margin: 0 auto;
        gap: 2rem;
    }
    .main-lower{
        background-color: rgb(2, 130, 249);
        color: white;
    }
    .card-lower{
        display: flex;
        align-items: center;
        padding: 1rem;
    }

    .card-lower img{
        width: 50%;
    }
    .card-lower *{
        margin-right: 0.6rem;
    }
</style>