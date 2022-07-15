<template>
  <section>
    <h4>
        {{ footerLists[0].title }}
    </h4>
    <ul>
        <li v-for="(element, index) in footerLists[0].content" :key="index">
            <a :href="element.ref">{{ element.name }}</a>
        </li>
    </ul>
  </section>
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

<style lang="scss" scoped>
    section {

        float: left;
        width: 30%;
        padding: 1rem;

        h4 {
            text-transform: uppercase;
            font-size: 2rem;
            color: white;
        }

        ul {
            list-style: none;

            li {
                a {
                    color: white;
                    text-decoration: none;
                }
            }
        }
    }
</style>