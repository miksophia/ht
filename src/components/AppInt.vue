<template>
  <div class="white-section section-arrow-top int">
    <div class="container container-cus">
      <div class="int-wrapper">
        <h2 class="t-white">
          Какие хостинг-компании мы рассматриваем в первую очередь?
        </h2>
        <div class="int__content">
          <p class="int__title">
            Преимуществом будут следующие факторы:
          </p>
          <ul class="list list-white-cus">
            <li v-for="item in intList" :key="item">
              {{item}}
            </li>
          </ul>
          <p class="description">
            Мы понимаем, что ваш проект может не соответствовать перечисленным пунктам. Они носят предпочтительный, а не обязательный характер. Будем рады пообщаться с вами лично и обсудить возможность индивидуального подхода при миграции ваших клиентов к нам на обслуживание.
          </p>
          <app-button>Оставьте ваши контакты</app-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      intList: [
        'Большая часть ваших клиентов - ИП и юридические лица',
        'Ваши тарифные планы близки по цене к нашим, или дороже их',
        'Используется панель управления хостингом cPanel',
        'Используется биллинговая система WHMCS',
        'Большинство клиентских доменов используют ваши DNS',
        'Вы используете собственные IP-адреса'
      ]
    }
  }
}
</script>

<style lang="scss">
  #app .section-arrow-top.int:before {
    background-image: url(./img/triangle.svg);
    background-repeat: no-repeat;
    background-size: 100% 100%;
    background-position: top center;
    content: '';
    display: block;
    width: 100%;
    height: 100px;
    margin-top: -100px;
    position: absolute;
    left: 0;
  }
  #app .int{
    background: #fff;
    position: relative;
  }
  .int-wrapper{
    padding-top: 80px;
    .t-white{
      font-weight: 600;
      font-size: 34px;
      line-height: 130%;
      text-align: center;
      color: #333333;
      padding-bottom: 60px;
    }
  }
  #app  .container.container-cus{
   padding: 0 15px;
  }
  #app .list.list-white-cus li:before{
    width: 10px;
    height: 10px;
    top: 8px;
  }
  #app .list.list-white-cus li{
    padding-left: 25px;
    margin-bottom: 10px;
    font-weight: 400;
    font-size: 18px;
    line-height: 150%;
    color: #333333;
  }
  .int__title{
    font-weight: 600;
    font-size: 20px;
    line-height: 120%;
    color: #333333;
    margin-bottom: 20px;
  }
  .int__content ul{
    margin-bottom: 20px;
  }
  .int__content .description{
    margin-bottom: 20px;
    font-weight: 400;
    font-size: 18px;
    line-height: 140%;
    color: #333333;
  }
</style>
