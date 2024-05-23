<script>
export default {
  data() {
    return {

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
            contenuto
        </section>
        <section class="main-lower">
            <div class="container">
                <div class="card">
                    <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/buy-comics-digital-comics.png" alt="buy-comics-digital-comics.png"> 
                    <p>DIGITAL COMICS</p>
                </div>
                <div class="card">
                    <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/buy-comics-merchandise.png" alt="buy-comics-digital-comics.png"> 
                    <p>DC MERCHANDISE </p>
                </div>
                <div class="card">
                    <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/buy-comics-subscriptions.png" alt="buy-comics-digital-comics.png"> 
                    <p>SUBSCRIPTION</p>
                </div>
                <div class="card">
                    <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/buy-comics-shop-locator.png" alt="buy-comics-digital-comics.png"> 
                    <p>COMIC SHOP LOCATOR</p>
                </div>
                <div class="card">
                    <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/buy-dc-power-visa.svg" alt=""> 
                    <p>DC POWER VISA</p>
                </div>
               
            </div>

        </section>

    </main>

</template>

<style scoped>
    .container{
        width: 1200px;
        display: flex;
        margin: 0 auto;
        gap: 2rem;
    }
.main-upper{
    background-color: rgb(28, 28, 28);
    color: white;
}
.main-lower{
    background-color: rgb(2, 130, 249);
    color: white;
}
.card{
    display: flex;
    align-items: center;
    padding: 1rem;
}

.card img{
    width: 50%;
}
.card *{
    margin-right: 0.6rem;
}
</style>