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