<template>
   <footer>
    <div class="container">
      <figure> <router-link :to="{name:'Home'}"><img src="@/assets/logo.svg" alt=""></router-link></figure>
      <ul>
        <li><router-link class="link" :to="{name:'Brand'}">品牌介紹</router-link></li>
        <li><a href="#">商品一覽</a></li>
        <li> <router-link class="link" :to="{name:'About'}">關於護膚</router-link></li>
        <li><a href="#">常見疑問</a></li>
        <li><a href="#">企業概要</a></li>
        <li><a href="#">聯絡方式</a></li>
      </ul>
      <ul>
        <li><a href="#">廣告一覽</a></li>
       
        <li><a href="#">隱私條款</a></li>
      </ul>
      <p>COPYRIGHT&copy; ION COSMETICS Co., Ltd. ALL RIGHTS RESERVED.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name:'Footer'
}
</script>

<style lang="scss" scoped>
footer {
  background: #eeeeee;
  padding: 3% 0 1.5%;
  figure {
    width: 17%;
    margin: auto;
  }
  ul {
    display: flex;
    width: 78%;
    margin: 5.5% auto;
    justify-content: space-between;

    li {
      position: relative;
      font-size: 20px;
      a {
        color: $black;
        font-weight: 600;
        &:hover {
          color: $mainColor;
        }
      }
      &:after {
        position: absolute;
        content: "/";
        color: #de1784;
        top: 20%;
        right: -42%;
        font-size: 12px;
      }
      &:last-child {
        &::after {
          display: none;
        }
      }
    }
    &:nth-of-type(2) {
      width: 23%;
      margin: 0 auto 1.8%;
      li {
        &:after {
          display: none;
        }
      }
    }
  }
  p {
    text-align: center;
    font-size: 14px;
    font-weight: 600;
    letter-spacing: 0.5px;
  }
}
</style>