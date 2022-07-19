<template>
  <footer>
    <div>
        <section class="footer-left">
          <FooterList v-for="(element, index) in footerLinks" :key="index"
            :title="element.title"
            :content="element.content" />
          

        </section>
        <section class="footer-right">

        </section>

    </div>
  </footer>
</template>

<script>

import FooterList from './FooterList.vue';


export default {

    
    components: {
        FooterList,
    },

    data: function() {
        return {

            footerLinks: 
            [
                {
                    title: "dc comics",
                    content: [
                        {
                            text: "Characters",
                            url: "#",
                        },
                        {
                            text: "Comics",
                            url: "#",
                        },
                        {
                            text: "Movies",
                            url: "#",
                        },
                        {
                            text: "TV",
                            url: "#",
                        },
                        {
                            text: "Games",
                            url: "#",
                        },
                        {
                            text: "Videos",
                            url: "#",
                        },
                        {
                            text: "News",
                            url: "#",
                        },
                    ]
                },
                {
                    title: "dc",
                    content: [
                        {
                            text: "Terms of use",
                            url: "#",
                        },
                        {
                            text: "Privacy policy (new)",
                            url: "#",
                        },
                        {
                            text: "Ad choices",
                            url: "#",
                        },
                        {
                            text: "Advertising",
                            url: "#",
                        },
                        {
                            text: "Jobs",
                            url: "#",
                        },
                        {
                            text: "Subscriptions",
                            url: "#",
                        },
                        {
                            text: "Talent workshops",
                            url: "#",
                        },
                        {
                            text: "CPSC certificates",
                            url: "#",
                        },
                        {
                            text: "Ratings",
                            url: "#",
                        },
                        {
                            text: "Shop help",
                            url: "#",
                        },
                        {
                            text: "Contact us",
                            url: "#",
                        },
                        
                    ]
                },  
                {
                    title: "sites",
                    content: [
                        {
                            text: "DC",
                            url: "#",
                        },
                        {
                            text: "MAD Magazine",
                            url: "#",
                        },
                        {
                            text: "DC Kids",
                            url: "#",
                        },
                        {
                            text: "DC Universe",
                            url: "#",
                        },
                        {
                            text: "DC Power Visa",
                            url: "#",
                        },
                    ]
                },
                {
                    title: "shop",
                    content: [
                        {
                            text: "Shop DC",
                            url: "#",
                        },
                        {
                            text: "Shop DC Collectibles",
                            url: "#",
                        },
                    ]
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../assets/stiles/variables.scss";
@import "../assets/stiles/mixins.scss";

  footer {

    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;

    &>div {
        @include generalContainer;
        display: flex;
        justify-content: space-between;
        height: 100%;

        .footer-left {
            width: 40%;
            padding: 4rem 0;
            display: flex;
            flex-wrap: wrap;

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