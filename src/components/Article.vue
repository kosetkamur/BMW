<template>
  <div class="articles">
    <div class="article" v-for="article_link in article_links">
      <div class="article__title">
        {{article_link}}
      </div>
      <div class="article__arrow"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      article_links: [
        'Page variation', 'Layout', 'Content'
      ]
    }
  }
}
</script>

<style>
  .articles{
    padding: 5px 0 5px 7px;
    width: 218px;
    height: 100%;
    min-height: 80vh;
    border-right: 1px solid #d6d6d6;
  }
  .article{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    border-bottom: 1px solid #e0e0e0;
    padding: 0 10px 1px 0;
    margin-bottom: 6px;
  }
  .article__title{
    font-size: 14px;
  }
  .article__arrow{
    background-image: url("../assets/images/icons/arrow_down.png");
    background-size: 23px 21px;
    background-repeat: no-repeat;
    background-position: center;
    color: #494949;
    width: 23px;
    height: 21px
  }
</style>