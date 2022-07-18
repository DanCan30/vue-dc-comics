<template>
  <div class="jumbo-container">
    <img src="../assets/img/jumbotron.jpg" alt="Comic Jumbotron">
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    div.jumbo-container {
        height: 35rem;
        width: 100%;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: top;
        }
    }

</style>