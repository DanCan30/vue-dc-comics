<template>
  <footer>
    <div>
        <section class="footer-left">
          <div v-for="(list, index) in footerLists" :key="index">
          <h3>
            {{list.title}}
          </h3>
          <ul>
            <li v-for="(element, index) in footerLists[index].content" :key="index">
              <a :href="element.ref">{{ element.name }}</a>
            </li>
          </ul>
          </div>
        </section>
        <section class="footer-right">

        </section>

    </div>
  </footer>
</template>

<script>

export default {

 data: function() {
        return {

            footerLists: 
            [
                {
                    title: "dc comics",
                    content: [
                        {
                            name: "characters",
                            ref: "#",
                        },
                        {
                            name: "comics",
                            ref: "#",
                        },
                        {
                            name: "movies",
                            ref: "#",
                        },
                        {
                            name: "TV",
                            ref: "#",
                        },
                        {
                            name: "games",
                            ref: "#",
                        },
                        {
                            name: "videos",
                            ref: "#",
                        },
                        {
                            name: "news",
                            ref: "#",
                        },
                    ]
                },
                {
                    title: "dc",
                    content: [
                        {
                            name: "terms of use",
                            ref: "#",
                        },
                        {
                            name: "privacy policy (new)",
                            ref: "#",
                        },
                        {
                            name: "ad choices",
                            ref: "#",
                        },
                        {
                            name: "advertising",
                            ref: "#",
                        },
                        {
                            name: "jobs",
                            ref: "#",
                        },
                        {
                            name: "subscriptions",
                            ref: "#",
                        },
                        {
                            name: "talent workshops",
                            ref: "#",
                        },
                        {
                            name: "CPSC certificates",
                            ref: "#",
                        },
                        {
                            name: "ratings",
                            ref: "#",
                        },
                        {
                            name: "shop help",
                            ref: "#",
                        },
                        {
                            name: "contact us",
                            ref: "#",
                        },
                        
                    ]
                },
                
                {
                    title: "sites",
                    content: [
                        {
                            name: "DC",
                            ref: "#",
                        },
                        {
                            name: "MAD Magazine",
                            ref: "#",
                        },
                        {
                            name: "DC Kids",
                            ref: "#",
                        },
                        {
                            name: "DC Universe",
                            ref: "#",
                        },
                        {
                            name: "DC Power Visa",
                            ref: "#",
                        },
                    ]
                },
                {
                    title: "shop",
                    content: [
                        {
                            name: "Shop DC",
                            ref: "#",
                        },
                        {
                            name: "Shop DC Collectibles",
                            ref: "#",
                        },
                    ]
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../stiles/variables.scss";
  @import "../stiles/mixins.scss";

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

            div {
              width: calc(100% / 3);

              h3 {
                text-transform: uppercase;
                color: $brandSecondaryColor;
                margin-bottom: 1rem;
                font-size: 1.5rem;
                letter-spacing: 2px;
              }

              ul {
              list-style: none;

                li {

                  a {
                    color: $textColor;
                    text-decoration: none;

                  &:hover {
                    color: $brandSecondaryColor;
                  }

                  }

                }
              }
            }
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