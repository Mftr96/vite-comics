<script>
export default {
  data() {
    return {
      dcComics:[
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      Dc:[
        "Terms Of Use",
        "Privacy policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites:[
        "DC",
        "MAD Magazine",
        "DC Kids",
        "DC Universe",
        "DC Power Visa"
      ],
    }
  },
  methods: {
    //funzioni Vue 
  },
  mounted() {
    console.log("App montata Footer");
  }
}

</script>
<template>
  <footer>
    <div class="footer-left">
        <div class="column">
          <h3>DC COMICS</h3>
          <p v-for="link in dcComics">{{link}}</p>
          <h3>SHOP</h3>
          <p>Shop Dc</p>
          <p>Shop DC Collectibles</p>

        </div>
        <div class="column">
          <h3>DC</h3>
          <p v-for="link in Dc">{{link}}</p>

        </div>
        <div class="column">
          <h3>SITES</h3>
          <p v-for="link in sites">{{ link }}</p>

        </div>
    </div>
    <div class="footer-right">
      <img src="../../src/assets/img/dc-logo-bg.png" alt="">
    </div>
  </footer>

</template>

<style scoped>
footer{
  width: 100%;
  height: 500px;
  background-image: url(../../src/assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: space-around;
  color: rgb(137, 126, 124);
}
h3{
  color: white;
}
p{
  margin-bottom: 0.3rem;
}
img{
  width: 100%;
}
.footer-left{
  display: flex;
  gap: 0.5rem;
}
.footer-right{
}
</style>