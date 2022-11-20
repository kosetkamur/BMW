<template>
  <div class="menu">
    <router-link to="/" class="menu__link title examples">Examples</router-link>
    <router-link to="/" class="menu__link title documentation">Documentation</router-link>
    <router-link to="/" class="menu__link title navigation">Navigation Examples</router-link>
    <div class="menu__link"></div>
  </div>
</template>

<style>
.menu{
  display: flex;
  flex-direction: row;
  padding: 0 5px;
  width: 100%;
  min-width: 934px;
  height: 25px;
  margin-bottom: 55px;
}
.menu__link{
  display: block;
  height: 25px;
  margin-right: 5px;
  border-bottom: 5px solid #d6d6d6;
  width: 130px;
  min-width: 130px;
}
.menu__link:last-child{
  width: 100%;
}
.title{
  font-family: BMWGroupTNCondensedTT-Regular,sans-serif;
  Font-size: 13px;
  color: #444444;
  text-align: center;
  text-decoration: none;
}
.menu__link.examples{
  display: block;
  height: 25px;
  border-bottom: 5px solid #035970;
  width: 228px;
  min-width: 228px;
}
</style>