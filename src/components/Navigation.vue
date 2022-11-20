<template>
  <div  class="nav">
      <router-link to="/" class="nav__btn home"></router-link>
      <router-link to="/" class="nav__btn help"></router-link>
      <router-link to="/" class="nav__btn mail"></router-link>
      <router-link to="/" class="nav__btn phone"></router-link>
      <router-link to="/" class="nav__btn info_btn"></router-link>
      <router-link to="/" class="nav__btn pen"></router-link>
      <div class="nav__lan">
        <div class="language">
          <div class="language__title">EN</div>
          <div class="language__arrow">
            <img alt="кнопка ручки" src="../assets/images/icons/arrow_down.png" class="arrow">
          </div>
        </div>
      </div>
      <router-link to="/" class="nav__btn search"></router-link>
      <router-link to="/" class="nav__btn logout"></router-link>
<!--    <router-view/>-->
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.nav{
  display: flex;
  flex-direction: row;
}
.nav__btn{
  display: block;
  color: #494949;
  height: 25px;
  width: 24px;
  vertical-align: middle;
  padding: 0 4px;
}
.nav__lan{
  color: #494949;
  margin: 0 4px;
}
.arrow{
  width:24px;
}
.language__title{
  font-family: BMWGroupTNCondensedTT-Regular, sans-serif;
}
.nav__btn::before{
  content: " ";
  border-left: 1px solid #eeefea;
  display: block;
  width: 1px;
  height: 24px;
  margin-left: -5px;
}
.nav__btn.help::before{
  content: " ";
  border-left: 1px solid #eeefea;
  display: block;
  width: 1px;
  height: 24px;
  margin-left: -5px;
}
.nav__btn.pen::after{
  content: " ";
  border-left: 1px solid #eeefea;
  display: block;
  width: 1px;
  height: 24px;
  margin-left: 27px;
  margin-top: -24px;
}
.nav__btn.pen::before{
  content: " ";
  border-left: 1px solid #eeefea;
  display: block;
  width: 1px;
  height: 24px;
  margin-left: -5px;
}
.nav__btn.home{
  background: url("../assets/images/icons/home.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.help{
  background: url("../assets/images/icons/help.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.mail{
  background: url("../assets/images/icons/mail.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.phone{
  background: url("../assets/images/icons/phone.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.info_btn{
  background: url("../assets/images/icons/info.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.pen{
  background: url("../assets/images/icons/pen.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.search{
  background: url("../assets/images/icons/search.png") center no-repeat;
  background-size: 24px auto;
}
.nav__btn.logout{
  background: url("../assets/images/icons/logout.png") center no-repeat;
  background-size: 24px auto;
}
.language{
  display: flex;
  flex-direction: row;
}
</style>
