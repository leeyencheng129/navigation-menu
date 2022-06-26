<template>
  <div id="warm" class="paddingTop">
    <div class="container">
      <section class="kv warm1">
        <div class="myrow">
          <div class="tx">
            <h2>溫泉熱蒸式美容法</h2>
            <h3>ION facial aesthetics</h3>
            <p>是利用『天然溫泉礦離子』的功效而開發的美容法，<br>使用毛巾充分善用熱度及水分美化原生肌膚。<br>
              是ION化妝品最有自信、強烈推薦的美容法。<br>
              維持美麗的第一步，正是維持“原生肌膚”的健康。
            </p>
          </div>
          <figure><img src="../assets/warm/warnup.png"></figure>
        </div>
      </section>

      <section class="content">
        <div class="myrow">
          <figure><img src="../assets/warm/warmup_01.jpg"></figure>
          <div class="tx">
            <div class="title">
              <div class="myrow">
                <div class="step">
                  STEP<span>1</span>
                </div>
                <div class="stepTx">清潔臉部</div>
              </div>

            </div>
            <p>
              將ION的CREAM SOAP用手掌搓揉充分起泡之後，輕柔緩慢地將泡泡完全包覆在臉部上進行清潔。<br>(建議使用溫水清潔)
            </p>
            <div class="txArea">
              <div class="myrow">
                <a href="/product/7/" class="text">礦離子卸妝洗面膏</a>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="content">
        <div class="myrow">
          <figure><img src="../assets/warm/warmup_02.jpg"></figure>
          <div class="tx">
            <div class="title">
              <div class="myrow">
                <div class="step">
                  STEP<span>2</span>
                </div>
                <div class="stepTx">面霜</div>
              </div>

            </div>
            <p>
              挑選適合肌膚的面霜，將面霜塗抹於全臉。
            </p>
            <div class="txArea">
              <div class="myrow">
                <a href="/product/2/" class="text">礦離子誘人保濕膏</a>
              </div>

            </div>
          </div>
        </div>
      </section>
      <section class="content">
        <div class="myrow">
          <figure><img src="../assets/warm/warmup_03.jpg"></figure>
          <div class="tx">
            <div class="title">
              <div class="myrow">
                <div class="step">
                  STEP<span>3</span>
                </div>
                <div class="stepTx">熱敷毛巾</div>
              </div>

            </div>
            <p>
              將毛巾(「溫泉熱蒸式美容法」專用毛巾)置於溫熱水中，稍微擰乾水分後，從臉包覆至頸部約1分鐘。
            </p>
            <div class="txArea">
              <div class="myrow">

              </div>

            </div>
          </div>
        </div>
      </section>
      <section class="content">
        <div class="myrow">
          <figure><img src="../assets/warm/warmup_04.jpg"></figure>
          <div class="tx">
            <div class="title">
              <div class="myrow">
                <div class="step">
                  STEP<span>4</span>
                </div>
                <div class="stepTx">按摩臉部</div>
              </div>

            </div>
            <p>
              取下毛巾後，用冷水打濕雙手，再將面霜置在臉上，以畫圓方式，由內往外側反覆進行臉部按摩，直到面霜被吸收。
            </p>
            <div class="txArea">
              <div class="myrow">

              </div>

            </div>
          </div>
        </div>
      </section>
      <section class="content">
        <div class="myrow">
          <figure><img src="../assets/warm/warmup_05.jpg"></figure>
          <div class="tx">
            <div class="title">
              <div class="myrow">
                <div class="step">
                  STEP<span>5</span>
                </div>
                <div class="stepTx">化妝水</div>
              </div>

            </div>
            <p>
              用水充分冷卻臉部後，請以輕拍方式塗上足量的化妝水至肌膚感受到滋潤保水為止。
              <br>
              如果您的皮膚較為敏感，或是擔心皮膚狀態不佳的話，請以雙手輕輕塗抹的方式進行。
            </p>

            <div class="txArea">
              <div class="myrow">
                <a href="/product/2/" class="text">礦離子誘人保濕膏</a>
                <a href="/product/4/" class="text">礦離子清爽化妝水</a>
              </div>

            </div>
          </div>
        </div>
      </section>

    </div>
  </div>
</template>

<script>
export default {
name:'About'
}
</script>

<style scoped lang="scss">
#warm {
  padding-bottom: 8%;
  .myrow {
    display: flex;
  }
  h2 {
    font-size: 30px;
    color: $mainColor;
    border-bottom: 1px solid $mainColor;
    width: fit-content;
    margin: 0 auto;
    line-height: 1.8;
    font-weight: 600;
  }
  h3 {
    line-height: 1.8;
    font-size: 24px;
  }

  .kv {
    padding-top: 8%;
    .tx {
      text-align: center;
      width: 50%;
    }
    figure {
      width: 60%;
      margin-left: -10%;
    }
    p {
      line-height: 2;
      margin-top: 3%;
      font-size: 16px;
    }
  }
  .warm1 {
    .myrow {
      align-items: center;
    }
  }
  .warm3 {
    img {
      width: 60%;
      margin-left: 30%;
    }
  }
  .content {
    margin: 7% 0;
    .tx {
      width: 50%;

      .step {
        width: 30%;
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
        font-size: 15px;
        span {
          font-size: 37px;
          padding-left: 5%;
          padding-bottom: 7%;
        }
        &:after {
          position: relative;
          content: "";
          height: 70%;
          width: 1px;
          top: 0;
          right: -20%;

          background: $mainColor;
        }
      }
      .stepTx {
        width: 70%;
        display: flex;
        align-items: center;
        padding-left: 5%;
        font-size: 30px;
      }
      p {
        border: 1px solid $mainColor;
        border-left: 0;
        height: 63%;
        display: flex;
        align-items: center;
        justify-content: center;
        line-height: 2;
        font-size: 18px;
        padding: 0 9%;
      }
    }
    figure {
      width: 50%;
    }
  }

  .title {
    color: $mainColor;
    height: 17%;
    border: 1px solid $mainColor;
    border-left: 0;
    border-bottom: 0;
    .myrow {
      height: 100%;
    }
  }
  .txArea {
    height: 20%;
    background: $mainColor;
    display: flex;
    align-items: center;
    padding: 0 5%;
    .text {
      color: #fff;
      width: 11.5vw;
      text-align: center;
      font-size: 1vw;
      display: block;
    }
  }
}

</style>