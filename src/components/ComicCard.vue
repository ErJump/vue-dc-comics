<template>
  <div class="col-2 comic-card mb-4">
    <img class="img-fluid mb-3" src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
    <h6 class="text-uppercase text-white">Action Comics</h6>
  </div>
</template>

<script>
export default {
  name: 'ComicCard',
  
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
