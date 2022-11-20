<template>
  <div class="menu">
    <div class="menu__meta">
      <div class="menu__logo"></div>
      <div class="menu__title">WEB USER INTERFACE</div>
    </div>
    <Navigation />
  </div>
</template>

<script>
import Navigation from '@/components/Navigation'
export default {
  name: "Header.vue",
  components: {
    Navigation
  }
}
</script>

<style scoped>
  .menu{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 12px 5px;
    margin-bottom: 20px;
  }
  .menu__title{
    font-family: BMWGroupTNCondensedTT-Regular, sans-serif;
    font-size: 33px;
    line-height: 26px;
    color: #444444;
  }
  .menu__meta{
    display: flex;
    flex-direction: row;
  }
  .menu__logo{
    background: url("../assets/images/logo.png") center no-repeat;
    background-size: 210px auto;
    width: 210px;
    height: 25px;
    margin-right: 23px;
  }
</style>