
<script>
//dall'export importo altri file vue
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppSocialFooter from './components/AppSocialFooter.vue';
export default {
  //componenti principali di vue:data,methods e mounted

  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppSocialFooter,
  },
  data() {
    return {
      nomeApplicazione: "VitEsempio 0.1"
    }
  },
  methods: {
    //vanno qui, al solito
  },
  mounted() {
    console.log("App montata");
  }
}
</script>


<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
  <AppSocialFooter/>
</template>

<style scoped>

</style>
