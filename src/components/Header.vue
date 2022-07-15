<template>
  <div>
    <header>
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
        <nav>

            <ul>
                <li v-for="(link, index) in navbarLinks" :key="index">
                    <a :href="link.href">
                        {{link.link}}
                    </a>
                </li>
            </ul>

        </nav>
    </header>
  </div>
</template>

<script>
export default {
    data: function() {
        return {

            navbarLinks: [
                {
                link: "characters",
                href: "#"
                },
                {
                link: "comics",
                href: "#"
                },
                {
                link: "movies",
                href: "#"
                },
                {
                link: "tv",
                href: "#"
                },
                {
                link: "games",
                href: "#"
                },
                {
                link: "collectibles",
                href: "#"
                },
                {
                link: "videos",
                href: "#"
                },
                {
                link: "fans",
                href: "#"
                },
                {
                link: "news",
                href: "#"
                },
                {
                link: "shop",
                href: "#"
                },
            ]

        }
    }
}
</script>

<style lang="scss" scoped>
  @import "../stiles/mixins.scss";
  @import "../stiles/variables.scss";


    header {
        @include generalContainer;
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            padding: 1.5rem 0;
        }
    }
    nav {
        
        ul {
            list-style: none;

            li {
                display: inline-block;
                
                a {
                    color: $textColor;
                    font-weight: bold;
                    text-decoration: none;
                    text-transform: uppercase;
                    padding: 3.65rem 1rem;

                    &:hover {
                        border-bottom: 5px solid $brandColor;
                        color: $brandColor;
                    }
                }
            }
        }
    }
        


</style>