<template>
   <section class="skinCare">
    <div class="container">
      <h2 class="myh2">您的肌膚問題</h2>
      <div class="content">
        <div class="mycard">
          <h3 class="pinkBB">粉刺煩惱</h3>
          <h4>Acne</h4>
          <p>粉刺的成因很複雜。<br>請使用正確的<br class="sp">洗臉產品以及護膚方式。<br>
            <span>※透過正確洗臉方式<br class="sp">可預防粉刺</span>
          </p>
        </div>
        <div class="mycard">
          <h3 class="pinkBB">年齡肌問題</h3>
          <h4>Aging</h4>
          <p>緊緻滋潤因皮膚表面水分不足而<br class="pc">彈性低下的肌膚。</p>
        </div>
        <div class="mycard">
          <h3 class="pinkBB">乾性肌膚</h3>
          <h4>Dry skin</h4>
          <p>即肌膚缺水的乾燥肌膚。<br class="pc">
            適合常年因皮膚乾燥而困擾的人。
          </p>
        </div>
        <div class="mycard">
          <h3 class="pinkBB">失去肌膚彈力</h3>
          <h4>Inelastic skin</h4>
          <p>想改善失去彈性的肌膚，<br class="pc">提高彈性及緊緻感。
          </p>
        </div>
        <div class="mycard">
          <h3 class="pinkBB">油性肌膚</h3>
          <h4>IOily skin</h4>
          <p>油性肌膚、<br>或有泛油光困擾。</p>
        </div>
        <div class="mycard">
          <h3 class="pinkBB">毛孔清潔問題</h3>
          <h4>Pore skin</h4>
          <p>徹底清除毛孔污垢，<br>緊緻肌膚、深度護膚。</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name:'Skin'
}
</script>

<style lang="scss" scoped>
.skinCare {
  background: url(../assets/bg.jpg) no-repeat;
  background-size: cover;
  background-position: top;
  padding: 2.5% 0;
  .content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .mycard {
    background: rgba(255, 255, 255, 0.918);
    width: 49%;
    text-align: center;
    height: 266px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin-bottom: 2%;

    h3 {
      width: fit-content;
      margin: 0 auto;
      line-height: 2;
      font-size: 24px;
    }
    h4 {
      color: $mainColor;
      font-size: 19px;
      line-height: 2;
      font-weight: 500;
    }
    p {
      font-size: 18px;
      font-weight: 500;
      margin-top: 2px;
      span {
        font-size: 16px;
        color: #949494;
      }
    }
  }
}
</style>