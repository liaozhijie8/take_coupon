<template>
  <van-nav-bar title="红包领取页" fixed left-arrow class="navbar-set" @click-left="onClickLeft" />
  <div class="coupon-container">
    <div class="top">
      <van-icon name="gold-coin-o" />中国银行
    </div>
    <div class="botton">
      <div class="price">
        <div><span style="font-size:30px">10.00元</span></div>
        <div><span>订单满100.00元使用</span></div>
      </div>
      <van-button round type="primary" class="button-set">立即领取</van-button>
      <div class="tip">
        <p>此红包为银行自行发放，仅限该银行渠道支付时使用</p>
        <p>请在2022.07.12 00:00:00~2022.07.13 23:59:59时间范围内领取</p>
      </div>
      <van-divider class="divider-set" dashed></van-divider>
      <div class="classifyItem">
        <p>有效期</p>
        <p>领取<span>2</span>天后有效</p>
      </div>
      <van-divider class="divider-set" />
      <div class="classifyItem">
        <p>适用商户及门店</p>
        <p><a href="#">查看商户及门店
            <van-icon name="arrow" />
          </a></p>
      </div>
      <van-divider class="divider-set" />
      <div class="classifyItem">使用规则</div>
      <div class="rule-detail">
        <span>(一) 活动时间</span>
        <p>1、北京时间：2022年07月12日00:00:00.2022F07#13 E 23:59:59,</p>
        <span>(二) 参与条件</span>
        <p>1、本活动仅限中华人民共和国境内（仅为本规
          则之目的，为避免疑义，不包括香港特别行政
          区、澳门特别行政区和台湾地区）
          （简称“中国
          境内〞）的支付宝实名认证的用户参加，未实名
          认证用户可至支付宝APP-我的-点击我的头像-选
          择身份认证完成认证后参与本活动。</p>
        <p>
          2、支付宝实名认证用户需绑定中国境内手机号
          码且手机号码有效。如用户支付宝账号绑定的手
          机号为港!澳/台/国外手机号，则无法参与。
        </p>
        <p>
          3、本活动仅限鄉定相关活动银行的银行卡的支付宝用户参与，如用户未绑定相关活动银行的银行卡，可至支付宝APP-我的-银行卡先行绑卡后参与。
        </p>
        <p>
          4、具体参与条件以各银行实际活动开展情况为
          准
        </p>
        <span>(三) 活动规则</span>
        <p>
          1、活动期间，符合本活动参与条件的用户在指
          定的活动页面，可以领取相关活动银行支付宝快
          捷支付满减红包 （以下简称满减红包)
        </p>
        <p>
          2、本次活动可领取的满减红包包括：
          （1） “中国银行信用卡满100.00元最多减10.00
          元红包"50份。
        </p>

      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'coupon-take',
  setup() {
    const onClickLeft = () => {
      alert('返回上级')
    }
    return {
      onClickLeft
    }
  }
})
</script>

<style lang="less" scoped>
// .navbar-set{
//   background-color: rgba(0, 0, 0, 0);
// }
body {
  background-color: red;
}

.coupon-container {
  text-align: center;
  margin: 50px 10px;

  .top {
    padding-left: 10px;
    line-height: 50px;
    text-align: left;
    height: 50px;
    background-color: rgb(243, 238, 238);
    border-radius: 5px;
    border-bottom-left-radius: 15px;
    border-bottom-right-radius: 15px;
  }

  .botton {
    padding: 5px 10px 5px;
    border-radius: 5px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
    background-color: white;

    .price {
      div {
        margin: 10px 0;
      }
    }

    .button-set {
      width: 80vw;
      height: 40px;
      background-color: rgb(56, 117, 245);
    }

    .tip {
      p {
        font-size: 12px;
      }
    }

    .divider-set {
      color: rgb(218, 218, 218);
      border-color: rgb(218, 218, 218);
    }

    .classifyItem {
      text-align: left;
      font-weight: bold;
      font-size: 16px;

      p {
        display: block;
      }

      p:first-child {
        border-left: 4px solid #3876fe;
        padding-left: 8px;
      }

      p:last-child {
        font-size: 14px;
        font-weight: normal;
        padding-left: 12px;
      }
    }

    .rule-detail {
      margin-top: 10px;
      text-align: left;
      font-size: 14px;

      span {
        display: block;
        text-indent: 1em;
      }

      p {
        margin: 0;
      }
    }
  }

}
</style>
