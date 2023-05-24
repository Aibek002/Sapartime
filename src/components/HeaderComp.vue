
<template>
  <header>
    <div class="item">
      <img src="https://github.com/Aibek002/SapaTime/blob/main/src/img/logotype.png?raw=true" alt="logo">
    </div>
    <div class="item"><a href="">Home</a></div>
    <div class="item"><a href="">About</a></div>
    <div class="item"><a href="">Listing</a></div>
    <div class="item"><a href="">Car</a></div>
    <div class="item"><a href="">Pages</a></div>
    <div class="item"><a href="">Contact</a></div>
    <div class="item"></div>
    <div class="item">
      <a  @click.prevent="toggleCurrency" href="">{{ currency }}</a>
    </div>
    <div class="item">
      <a href=""><img src="https://t4.ftcdn.net/jpg/04/87/76/53/240_F_487765314_EWxEN4PaEjMDGbtep3zpNx2VUPJQAtWG.jpg" class="shopIcon" alt=""></a>
    </div>
    <div class="item">
      <a href=""><img src="https://cdn-icons-png.flaticon.com/128/310/310869.png" class="loginIcon" alt=""></a>
    </div>
  </header>
  <h1>{{ currency }}</h1>
</template>

<script>
export default {
  data() {
    return {
      usd: [22, 33, 55, 222, 1, 3, 5, 5, 6, 2, 1],
      euro: [21, 2, 4, 5, 3, 2, 2, 4, 5, 5, 1, 2, 3],
      currency: 'USD'
    };
  },
  methods: {
    toggleCurrency() {
      this.currency = this.currency === 'USD' ? 'EURO' : 'USD';
    }
  }
};
</script>


<style scoped>
header {
  display: grid;
  grid-template-columns: 25% 7% 7% 7% 5% 7% 20% 5% 5% 5%;
  grid-template-areas: 'item item . . . . . . . . .';
  height: 70px;
  border-bottom: 1px solid var(--light-grey-color,#EAEEF3);
  padding-top: 20px;
  line-height: 3;

}

header a {
  color: #232323;
  text-decoration: none;
  position: relative;
  font-weight: 700;
  font-size: 16px;
  font-family: dm sans,sans-serif;
}
header img{
  height: 50px;
  margin: 0;
}
.loginIcon{
  height: 30px;
  padding-top: 8px;
}
.shopIcon{
  height: 30px;
  padding-top: 8px;

}
</style>
