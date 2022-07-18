<template>
  <div class="bg-main">
    <div class="py-5">
      <div class="container-lg">
        <h3 class="text-white">Content goes here</h3>
      </div>
    </div>
    <div class="bg-sec py-5">
      <div class="container-lg">
        <div class="row justify-content-around">
          <div v-for="(element, index) in productsList" :key="index" class="col-2 d-flex justify-content-center align-items-center">
            <img  class="w-25" :src="`/img/${element.img}`" :alt="element.name">
            <h5 class="text-uppercase text-white ms-2 fs-6">{{element.name}}</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContentMain',
  data: function(){
    return {
      productsList: [
        {
          name: "digital comics",
          img: "buy-comics-digital-comics.png",
        },
        {
          name: "dc merchandise",
          img: "buy-comics-merchandise.png",
        },
        {
          name: "subscription",
          img: "buy-comics-subscriptions.png",
        },
        {
          name: "comic shop locator",
          img: "buy-comics-shop-locator.png",
        },
        {
          name: "dc power visa",
          img: "buy-dc-power-visa.svg",
        },
      ],
      imgPath: require("../assets/img/buy-comics-digital-comics.png"),
    }
  },
  methods: {
    completeImgPath: function(img){
      return "@/assets/img/" + img + ".png";
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../assets/styles/variables.scss";
  .bg-main{
    background-color: $fontColor;
  }
  .bg-sec{
    background-color: $brandColor;
  }
</style>
