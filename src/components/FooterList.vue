<template>

    <div>
        <h3>
            {{title}}
          </h3>
          <ul>
            <li v-for="(element, index) in content" :key="index">
              <a :href="element.url">{{ element.text }}</a>
            </li>
          </ul>
    </div>

</template>

<script>
export default {

    props: {
        title: String,
        content: Array,
    }
   
}
</script>

<style lang="scss" scoped>

@import "../assets/stiles/variables.scss";

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

</style>