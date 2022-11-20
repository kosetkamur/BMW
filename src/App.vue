<template>
  <Header />
  <Menu />
  <Home />
</template>


<style>
@import 'assets/fonts/fonts.css';

*{
  font-family: BMWGroupTNCondensedTT-Regular, sans-serif;
}
</style>
<script>
import Header from '@/components/Header'
import Menu from '@/components/Menu'
import Home from '@/views/Home'

export default {
  components: {Header, Menu, Home}
}
</script>