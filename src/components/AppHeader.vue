<script>
export default {
  data() {
    return {
        headerList:[
            "CHARACTERS",
            "COMICS",
            "MOVIES",
            "TV",
            "GAMES",
            "COLLECTIBLES",
            "VIDEOS",
            "FANS",
            "NEWS",
            "SHOP",
        ]
    }
  },
  methods: {
    //funzioni Vue 
  },
  mounted() {
    console.log("App montata Header");
  }
}
</script>

<template>
    <header>
        <img src="../../vue-dc-comics-1/vue-dc-comics-1/img/dc-logo.png" alt="dc-logo.png">
        <div class="header-right">
            <a v-for="link in headerList" href="#">{{link}}</a>
        </div>

    </header>

</template>

<style scoped>
header{
    display: flex;
    justify-content: space-around;
    padding: 2rem;
}

.header-right{
    padding: 0.3rem;
    display: flex;
    align-items: center;
    gap: 0.4rem;

}
</style>