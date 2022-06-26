<template>
  <section class="beauty">
    <div class="container">
      <div class="h2Box">
        <h2 class="myh2">ION美容法</h2>
      </div>
      <p>ION化妝品是以溫泉中含有的<br class="sp">16種天然礦物質離子為基礎，<br>並添加有效的天然保濕成分，<br class="sp">是使讓肌膚保持美麗、健康狀態的保養品。<br>
        只要每天正確使用，<br class="sp">打好基礎就能引導肌膚恢復健康。<br class="sp">請開跟著我們始保養的第一步吧!</p>

      <div class="content">
        <div class="mycard">
          <div class="tx">
            <h3 class="pinkBB">溫泉熱蒸式美容法</h3>
            <article>
              <p>
                ION自信推薦的美容法。<br class="pc">利用「天然溫泉礦物質離子」的功效而開發的保養方式，<br>使用溫熱毛巾及水分使原生肌膚變得美麗。
              </p>
              <p>維持美麗的第一步，正是維持“原生肌膚”的健康。</p>
            </article>
            <a href="#" class="Btn pinkBtn">MORE</a>
          </div>
          <figure><img src="../assets/beauty_01.jpg"></figure>
        </div>
        <div class="mycard">
          <div class="tx">
            <h3 class="pinkBB">溫泉式光滑美容法</h3>
            <article>
              <p>
                早晨總是匆匆忙忙。
              </p>
              <p>但，一早的保養是必要不可少的。<br>溫泉式光滑美容法非常適合這樣忙碌的您</p>
            </article>
            <a href="#" class="Btn pinkBtn">MORE</a>
          </div>
          <figure><img src="../assets/beauty_02.jpg"></figure>
        </div>
        <div class="mycard">
          <div class="tx">
            <h3 class="pinkBB">簡單魅力美容法</h3>
            <article>
              <p>
                初生時帶有迷人光采的肌膚，<br>
                在進入青春期就開始會遇到各式各樣的考驗。<br>
                為了保持水嫩的肌膚，<br>
                從年輕時期就要開始好好地做足基礎美容。
              </p>
            </article>
            <a href="#" class="Btn pinkBtn">MORE</a>
          </div>
          <figure><img src="../assets/beauty_03.jpg"></figure>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name:'Beauty'
}
</script>

<style lang="scss" scoped>
.beauty {
  background: url(../assets/bg2.jpg) no-repeat;
  background-size: cover;
  background-position: center;
  padding: 2% 0 5%;
  p {
    text-align: center;
    font-size: 18px;
    margin: 4% 0 5%;
    font-weight: 500;
  }

  .mycard {
    display: flex;
    background: #fff;
    margin-bottom: 3%;
    .tx {
      width: 50%;
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      h3 {
        font-size: 24px;
        color: $mainColor;
        width: fit-content;
        margin: 0 auto;
        line-height: 1.8;
      }
      article {
        margin: 3% 0 5%;
      }
      p {
        font-size: 16px;
        margin: 0;
      }
    }
    figure {
      width: 50%;
    }
    &:nth-child(2n) {
      flex-direction: row-reverse;
    }
  }
}
</style>