<template>
  <div>
    <header>
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
        <nav>

            <ul>
                <li v-for="(headerLink, index) in navbarLinks" :key="index">
                    <a :href="headerLink.href" 
                        :class="{active: headerLink.selected === true}">
                        {{headerLink.link}}
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
                href: "#",
                selected: false,
                },
                {
                link: "comics",
                href: "#",
                selected: true,
                },
                {
                link: "movies",
                href: "#",
                selected: false,
                },
                {
                link: "tv",
                href: "#",
                selected: false,
                },
                {
                link: "games",
                href: "#",
                selected: false,
                },
                {
                link: "collectibles",
                href: "#",
                selected: false,
                },
                {
                link: "videos",
                href: "#",
                selected: false,
                },
                {
                link: "fans",
                href: "#",
                selected: false,
                },
                {
                link: "news",
                href: "#",
                selected: false,
                },
                {
                link: "shop",
                href: "#",
                selected: false,
                },
            ]

        }
    }
}
</script>

<style lang="scss" scoped>
  @import "../assets/stiles/mixins.scss";
  @import "../assets/stiles/variables.scss";


    header {
        @include generalContainer;
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            padding: 1.5rem 0;
        }
    }

        
    nav ul {
        list-style: none;

        li {
            display: inline-block;
            margin: 0 1rem;
            
            a {
                color: $textColor;
                font-weight: bold;
                text-decoration: none;
                text-transform: uppercase;
                padding: 3.65rem 0;

                &:hover,
                &.active {
                    border-bottom: 5px solid $brandColor;
                    color: $brandColor;
                }
            }
        }
    }
    


</style>