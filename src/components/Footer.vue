<template>
  <footer>
    <div>
        <section class="footer-left">

            <FooterElementList />
            <FooterElementList />
            <FooterElementList />
            <FooterElementList />

        </section>
        <section class="footer-right">

        </section>

    </div>
  </footer>
</template>

<script>
import FooterElementList from './FooterList.vue';

export default {

    components: {
        FooterElementList,
    }

}
</script>

<style lang="scss">
  @import "../stiles/mixins.scss";

  footer {

    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;

    div {
        @include generalContainer;
        display: flex;
        justify-content: space-between;
        height: 100%;

        .footer-left {
            width: 35%;
        }

        .footer-right {
            width: 40%;
            background-image: url("../assets/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;

        } 
    }
  }

</style>