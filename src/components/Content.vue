<template>
  <main>
    <div>
        <h2> --- Content goes here --- </h2>
    </div>
  </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  @import "../stiles/mixins.scss";
  @import "../stiles/variables.scss";

    main {
        background-color: #1C1C1C;

        div {
            @include generalContainer;
            color: $brandSecondaryColor;

            h2 {
              font-size: 2.1rem;
                padding: 6rem 0;
            }
        }
    }
</style>