<template>
  <div id="app">
    <HeaderMain/>
    <ContentMain/>
    <FooterMain/>
  </div>
</template>

<script>
import ContentMain from './components/ContentMain.vue';
import HeaderMain from './components/HeaderMain.vue';
import FooterMain from './components/FooterMain.vue';

export default {
  name: 'App',
  components: {
    ContentMain,
    HeaderMain,
    FooterMain,
  }
}
</script>

<style lang="scss">
  @import "assets/styles/variables.scss";
  @import "~bootstrap/dist/css/bootstrap.css";

  *{
    /* outline: 1px solid red; */
  }


</style>
