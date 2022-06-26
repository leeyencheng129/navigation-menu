<template>
  <div id="contact" class="paddingTop">

    <div class="container">
      <div class="myrow">
        <section>
          <h2>聯繫我們</h2>

          <p>關於在ION Kesho網路商店購買的產品以及使用方法，若有任何問題，歡迎使用郵件與我們聯繫。<br>為節省您寶貴的時間，詢問前請先參閱<a href="/faq">「常見疑問」</a>確認。<br>
            此外，此諮詢窗口為麗溫化妝品 ION Kesho網路商店之專用窗口，此網路商店以外的諮詢恕無法回覆，造成不便敬請見諒。
          </p>
        </section>
        <section>
          <h3>【郵件諮詢】</h3>
          <p>我們將按照客戶聯繫的順序進行回覆，敬請稍後。<br>如果您使用免費郵件(Yahoo! Mail，Gmail等)，回覆郵件時有可能被分類到垃圾信件中，請知悉。<br>
            若要採取措施防止回信變成垃圾郵件，請在您的信箱系統內解除<a
              href="mailto:kazuki_mikashima@brangista.com"><span>kazuki_mikashima@brangista.com</span></a>為垃圾郵件。<br>（若未解除，將可能無法收到本公司所寄送的聯絡事項。）<br>
            ※電子郵件無法傳遞時，客服人員可能會以電話方式與您聯繫，請知悉。
          </p>
        </section>

        <section>
          <p class="contactBtn"><a href="mailto:kazuki_mikashima@brangista.com">客服郵件：kazuki_mikashima@brangista.com</a>
          </p>
          <p>(週末、國定假日等期間，客服將暫停服務，敬請見諒。)</p>
        </section>
      </div>

    </div>



  </div>
</template>

<script>
export default {
name:'Contact'
}
</script>

<style scoped lang="scss">
#contact {
  letter-spacing: 1;
  h2,
  h3 {
    margin-bottom: 1.5%;
  }
  h2 {
    font-size: 32px;
  }
  h3 {
    font-size: 28px;
  }
  p {
    font-size: 16px;
    line-height: 1.8;
  }
  .myrow {
    padding: 8% 0;
  }
  section {
    + section {
      margin-top: 5%;
    }
  }
  a {
    color: $mainColor;
  }
  .contactBtn {
    background: $mainColor;
    width: fit-content;
    padding: 2% 3%;
    a {
      color: #fff;
      font-weight: 700;
    }
  }
}
@media screen and (max-width: 1440px) {
  #contact {
    h2 {
      font-size: 2vw;
    }
    h3 {
      font-size: 1.8vw;
    }
    p {
      font-size: 1.2vw;
    }
  }
}
</style>