<template>
  <div class="col-2 comic-card mb-4">
    <img class="img-fluid mb-3" :src="object.thumb" :alt="object.series">
    <h6 class="text-uppercase text-white">{{object.series}}</h6>
  </div>
</template>

<script>
export default {
  name: 'ComicCard',
  props: {
    object: {
      type: Object,
      required: true
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../assets/styles/variables.scss";
  
  img{
    object-fit: cover;
    height: 200px;
    width: 100%;
    object-position: top;
  }
</style>
