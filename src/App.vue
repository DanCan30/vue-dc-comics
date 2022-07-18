<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Content />
    <Store />
    <Footer />
    <Socials />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Jumbotron from './components/Jumbotron.vue';
import Content from './components/Content.vue';
import Store from './components/Store.vue';
import Footer from './components/Footer.vue';
import Socials from './components/Socials.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Content,
    Store,
    Footer,
    Socials,
  }
}
</script>

<style lang="scss">

  @import "./assets/stiles/common.scss";
  @import "./assets/stiles/mixins.scss";
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;500;700;900&display=swap');


</style>
