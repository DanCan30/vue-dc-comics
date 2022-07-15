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

    main {
        background-color: #1C1C1C;

        div {
            @include generalContainer;
            color: white;

            h2 {
                padding: 5rem 0;
            }
        }
    }
</style>