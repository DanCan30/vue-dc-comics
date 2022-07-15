<template>
    <section>
        <div>
            <ul>
                <li v-for="(element, index) in storeInfos" :key="index">
                    <img :src="`../../bonus-images/buy-${element.imgSrc}`" :alt="element.text">
                    <a :href="element.ref">{{ element.text }}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {

    data: function() {
        return {

        storeInfos: [
            {
                imgSrc: "comics-digital-comics.png",
                text: "digital comics",
                ref: "#",
            },
            {
                imgSrc: "comics-merchandise.png",
                text: "merchandise",
                ref: "#",
            },
            {
                imgSrc: "comics-subscriptions.png",
                text: "subscriptions",
                ref: "#",
            },
            {
                imgSrc: "comics-shop-locator.png",
                text: "comic shop locator",
                ref: "#",
            },
            {
                imgSrc: "dc-power-visa.svg",
                text: "dc power visa",
                ref: "#",
            },
        ]
        }
    }

}
</script>

<style lang="scss" scoped>
    @import "../stiles/mixins.scss";
    @import "../stiles/variables.scss";


  section {
    background-color: $brandColor;

    div {
        @include generalContainer;

        ul {

            display: flex;
            justify-content: space-evenly;
            list-style: none;
            padding: 4rem 0;

            li {
                display: flex;
                align-items: center;

                img {
                    width: 4rem;
                }

                a {
                    text-decoration: none;
                    color: $brandSecondaryColor;
                    text-transform: uppercase;
                    margin-left: 2rem;
                    font-weight: normal;
                }
            }
        }
    }
  }


</style>