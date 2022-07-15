<template>
  <div id="app">
    <Header />
    <Content />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'
import Socials from './components/Socials.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Footer,
    Socials,


  }
}
</script>

<style lang="scss">

  @import "./stiles/common.scss";
  @import "./stiles/mixins.scss";
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;500;700;900&display=swap');


</style>
