<template>
  <div class="card">

    <div class="comic-img-container">
        <img :src="thumbnail" :alt="series">
    </div>
    <h4>{{ series }}</h4>

  </div>
</template>

<script>
export default {
    props: {
        thumbnail: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>

<style lang="scss" scoped>

  div.card {
    width: calc((100% / 6) - 6rem);
    margin: 3rem;

    h4 {
      text-transform: uppercase;
      font-size: .8rem;
    }


    .comic-img-container {
      width: 100%;

      
      img {
        width: 17rem;
        height: 17rem;
        object-fit: cover;
        object-position: top;
        margin-bottom: 1rem;
      }
    }

  }

</style>