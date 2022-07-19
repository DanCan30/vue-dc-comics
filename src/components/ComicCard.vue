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
    width: calc((100% / 6) - 2rem);
    margin: 1rem;

    h4 {
      text-transform: uppercase;
      font-size: .8rem;
      margin-top: 1rem;
    }


    .comic-img-container {
      width: 18rem;
      height: 18rem;
      overflow: hidden;

      
      img {
        cursor: pointer;
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
        transition: .3s;

        &:hover {
          transform: scale(1.2);
          filter: saturate(40%);
        }
      }
    }

  }

</style>