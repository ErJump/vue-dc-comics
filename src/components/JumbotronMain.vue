<template>
  <div class="jumbotron">
  </div>
</template>

<script>


export default {
  name: 'JumbotronMain',
  
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../assets/styles/variables.scss";
  .jumbotron {
    width: 100%;
    background-image: url(../../public/img/jumbotron.jpg);
    height: 500px;
    background-size: cover;
    background-position: top;
    background-repeat: no-repeat;
  }
</style>
