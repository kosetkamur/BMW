<template>
  <div class="home-page">
    <Article />
    <div class="wui-container">
      <div v-for="wui in wuis" class="wui__item">
        <h1>{{ wui.title }}</h1>
        <div class="info">
          <ul v-for="text in wui.texts" class="info__item">
            <li>
                <a v-bind:href="text.href">
                  {{ text.body }}
                </a>
            </li>
          </ul>
        </div>
      </div>
      <div class="footer">
        © Copyright 2022 BMW Group
      </div>
    </div>
  </div>
</template>

<script>

import Article from "@/components/Article";
export default {
  name: 'Home',
  components: {Article},
  data() {
    return {
      wuis: [
        {title: "Page variation examples", texts: [{href: '/', body: 'IFrame page / No left navigation'}]},
        {title: "Layout examples", texts: [{href: '/', body: '100% Layout'},{href: '/', body: '50%/50% Layout'},{href: '/', body: '66%/33% Layout'},{href: '/', body: '100% - 33%/33%/33% - 100% Layout'},]},
        {title: "Content examples", texts: [{href: '/', body: 'Tabs'}]},
      ]
    }
  }
}
</script>

<style>
.home-page{
  display: flex;
  flex-direction: row;
}
.wui-container{
  padding: 0 12px;
}
.wui__item::before{
  content: " ";
  display: block;
  height: 6px;
  background-color: #d6d6d6;
  margin-bottom: 13px;
  width: 100%;
  min-width: 1170px;
}
h1{
  color: #494949;
  font-size: 15px;
  font-family: BMWGroupTNCondensedProTT-Bold, sans-serif;
  background-color: transparent;
  margin: 0;
  padding: 3px 0;
  min-height: 24px;
}
.info__item a{
  color: black;
  text-decoration: underline;
  font-size: 13px;
  font-family: BMWGroupTNTT-Regular,sans-serif;
}
ul{
  margin: 0;
  padding-left: 29px;
  line-height: 17px;
}
.info{
  margin: 16px 0;
}
.footer{
  font-family: BMWGroupTNTT-Regular,sans-serif;
  color: #494949;
  padding-top: 15px;
  padding-bottom: 7px;
  font-size: 14px;
}
</style>
