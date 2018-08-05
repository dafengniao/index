<template>
  <div>
    <div :class="hasActive ? 'header active' : 'header'">
      <div class="nav">
        <div class="logo">
          <img class="img_logo" src="http://homepage.lexivip.com/images/logo2.png">
        </div>
      </div>
    </div>

    <div class="container">
      <!-- 轮播图 -->
      <div class="banner" ref="banner">
        <el-carousel :interval="5000" :height="scrrentHeight" arrow="never" :autoplay="true">
          <el-carousel-item>
            <img src="../assets/images/banner.jpg">
          </el-carousel-item>
          <el-carousel-item>
            <img src="http://homepage.lexivip.com/images/63.png">
          </el-carousel-item>
          <el-carousel-item>
            <img src="../assets/images/banner.jpg">
          </el-carousel-item>
        </el-carousel>
      </div>

      <div class="descrite" ref="descrite">
        <div class="descrite_inline">
          <img class="descrite_inline_img" src="../assets/images/pinzhi.png">
          <h2>品质保障</h2>
          <p>乐喜提供购物品质保障，精挑细选，原创品牌均采用邀请制</p>
        </div>
        <div class="descrite_inline">
          <img class="descrite_inline_img" src="../assets/images/danbao.png">
          <h2>乐喜担保交易</h2>
          <p>用户收到商品，确认收货后乐喜才付款给创作人</p>
        </div>
        <div class="descrite_inline">
          <img class="descrite_inline_img" src="../assets/images/shiming.png">
          <h2>创作人实名认证</h2>
          <p>创作人及原创品牌均经过乐喜身份证明文件实名认证</p>
        </div>
      </div>
      <div class="slider">
        <swiper :options="swiperOption">
          <!-- slides -->
          <swiper-slide>
            <div class="slider_left">
              <div class="phone_bg">
                <img class="swiper_bg" src="../assets/images/swiper_1.jpg" />
                <img src="../assets/images/swiper_p_1.png" class="swiper_p_1">
                <img src="../assets/images/swiper_p_2.png" class="swiper_p_2">
                <img src="../assets/images/swiper_p_3.png" class="swiper_p_3">
                <img src="../assets/images/swiper_p_4.png" class="swiper_p_4">
              </div>
            </div>
            <div class="slider_right">
              <h2>有温度的社区优质内容服务</h2>
              <p>种草笔记，建立橱窗，塑造自己的独特风格。 </p>
              <p>聚焦创作人背后的故事，记录新奇好物创作的历程， </p>
              <p>将有温度的情感内容社交化的分发传播</p>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="slider_left">
              <div class="phone_bg">
                <img class="swiper_bg" src="../assets/images/swiper_1.jpg" />
                <img src="../assets/images/swiper_p_1.png" class="swiper_p_1">
                <img src="../assets/images/swiper_p_2.png" class="swiper_p_2">
                <img src="../assets/images/swiper_p_3.png" class="swiper_p_3">
                <img src="../assets/images/swiper_p_4.png" class="swiper_p_4">
              </div>
            </div>
            <div class="slider_right">
              <h2>有温度的社区优质内容服务</h2>
              <p>种草笔记，建立橱窗，塑造自己的独特风格。 </p>
              <p>聚焦创作人背后的故事，记录新奇好物创作的历程， </p>
              <p>将有温度的情感内容社交化的分发传播</p>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="slider_left">
              <div class="phone_bg">
                <img class="swiper_bg" src="../assets/images/swiper_1.jpg" />
                <img src="../assets/images/swiper_p_1.png" class="swiper_p_1">
                <img src="../assets/images/swiper_p_2.png" class="swiper_p_2">
                <img src="../assets/images/swiper_p_3.png" class="swiper_p_3">
                <img src="../assets/images/swiper_p_4.png" class="swiper_p_4">
              </div>
            </div>
            <div class="slider_right">
              <h2>有温度的社区优质内容服务</h2>
              <p>种草笔记，建立橱窗，塑造自己的独特风格。 </p>
              <p>聚焦创作人背后的故事，记录新奇好物创作的历程， </p>
              <p>将有温度的情感内容社交化的分发传播</p>
            </div>
          </swiper-slide>
          <!-- Optional controls -->
          <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
      </div>
      <div class="product">
        <div class="content">
          <div class="title">我们的产品</div>
          <div class="allitems">
            <div class="item s_1">
              <div class="word">
                <h2>乐喜品牌独立小程序</h2>
                <p>设计师，手作人，原创个人工作室品牌独立自主经营，沉淀客源，聚合社交流量。</p>
              </div>
            </div>
            <div class="item s_2">
              <div class="word">
                <h2>
                  <span>乐喜</span>
                  生活馆
                  <div class="hr"></div>
                </h2>
                <p>开启全民零售时代做自己热爱事，顺便赚取收入</p>
              </div>
            </div>
            <div class="item s_3">
              <div class="word">
                <h2>
                  <span>乐喜</span>
                  核心平台
                  <div class="hr"></div>
                </h2>
                <p>多元化和归属感是我们的立足之本。致力与构建原创，品质,和值得信任的全球品位社区</p>
              </div>
            </div>
            <div class="item s_4">
              <div class="word">
                <h2>
                  <span>乐喜</span>
                  PMS平台
                  <div class="hr"></div>
                </h2>
                <p>一站式管理订单、商品，物流乐喜全渠道分发，聚合线上线下销售</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="server">
        <div class="title">
          我们的服务
        </div>
        <div class="server_inline">
          <img src="../assets/images/saas.png">
          <h2>Saas平台服务</h2>
          <p>自建一站式全流程的Saas平台服务系统。 百万原创品牌便捷接入新零售场景。</p>
        </div>
        <div class="server_inline">
          <img src="../assets/images/quanqd.png">
          <h2>全渠道分发销售网络</h2>
          <p>我们建立和打通了百万独立品牌小程序，官方平台数据，与馆主，粉丝，客人，媒体建立分销网络，让百万sku商品轻松触达千万精准用户。</p>
        </div>
        <div class="server_inline">
          <img src="../assets/images/shequn.png">
          <h2>强大的社群与营销体系</h2>
          <p>我们利用构建的营销工具和营销策略，透过自有平台，小程序矩阵，社交体系，社群和自媒体的力量，实现精准引流和销售的增长</p>
        </div>
        <div class="server_inline">
          <img src="../assets/images/shouyint.png">
          <h2>乐喜收银台</h2>
          <p>基于线下场景流量聚合，将线下 创意市集，快闪店，体验店，库存一并轻松管理，提升交易经营效率，增加复购率</p>
        </div>
      </div>
      <div class="sym">
        <div class="content">
          <div class="cont">
            <h3>强大的小灵兽智慧零售系统</h3>
            <p>专注智慧零售技术服务，通过移动化、数据化、智能化的升级，帮助企业链接业务系统和外部大数据，有效提升零售行业“人·货·场”的效率，让万千企业快速实现智慧零售。</p>
            <div class="hr"></div>
          </div>
          <img src="../assets/images/sym_r.png">
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'Home',
  data () {
    return {
      scrrentHeight: '0px',
      hasActive: false,
      swiperOption: {
        direction: 'vertical',
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        }
      }
      // swiperOption: {
      //   notNextTick: true,
      //   autoplay: 3000,
      //   direction: 'vertical',
      //   grabCursor: true,
      //   setWrapperSize: true,
      //   autoHeight: true,
      //   pagination: {
      //     el: '.swiper-pagination',
      //     clickable :true
      //   },
      //   paginationClickable: true,
      //   mousewheelControl: true,
      //   observeParents: true,
      //   noSwiping: true,
      //   debugger: true
      // }
    }
  },
  components: {
    swiper,
    swiperSlide
  },
  mounted () {
    let scrrentWidth = document.documentElement.clientWidth
    if (scrrentWidth >= 1400) {
      this.$refs.banner.style.height = Math.ceil(scrrentWidth / 3.7) + 'px'
      this.scrrentHeight = Math.ceil(scrrentWidth / 3.7) + 'px'
    } else {
      this.scrrentHeight = this.$refs.banner.style.height = '378px'
    }
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll () {
      let scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop
      let offsetTop = this.$refs.descrite.offsetTop
      if (scrollTop >= offsetTop) {
        this.hasActive = true
      } else {
        this.hasActive = false
      }
    }
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less">
  .header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 80px;
    background: rgba(0,0,0,0);
    z-index: 999;
    &.active{
      background: #fff;
    }
    .nav{
      width: 100%;
      height: 80px;
      .logo{
        position: absolute;
        left: 30px;
        top: 20px;
        display: block;
        .img_logo{
          width: 148px;
          height: 40px;
        }
      }
    }
  }
  .bg_header{
    position: relative;
    width: 100%;
    height: 80px;
    background: transparent;
  }
  .el-carousel__arrow{
    display: none !important;
  }
  .el-carousel,.el-carousel__container{
    height: 100%;
    .el-carousel__item {
      height: 100%;
      img{
        width: 100% !important;
        min-width: 1400px;
      }
    }
    // 轮播按钮
    .el-carousel__indicators {
      .el-carousel__indicator{
        padding: 20px 6px !important;
        .el-carousel__button{
          width: 10px;
          height: 10px;
          border-radius: 10px;
        }
      }
    }
  }

  .descrite {
    margin: auto;
    width: 1180px;
    overflow: hidden;
    padding-top: 100px;
    .descrite_inline{
      float: left;
      width: 290px;
      text-align: center;
      margin: 0 50px;
      padding-bottom: 100px;
      .descrite_inline_img{
        width: 100px;
        height: 100px;
      }
      h2{
        font-size: 24px;
        margin-top: 18px;
      }
      p{
        font-size: 14px;
        color: #666666;
        margin-top: 10px;
        line-height: 26px;
      }
    }
  }

  .slider{
    height: 668px;
    margin: auto;
    width: 1180px;
    overflow: hidden;
    position: relative;
  }
  .swiper-container,.swiper-slide{
    height: 100%;
  }
  .slider_left{
    height: 598px;
    width: 402px;
    position: absolute;
    left: 0;
    top: 35px;
  }
  .phone_bg{
    width: 402px;
    height: 596px;
    position: absolute;
    top: 0;
    left: 50px;
    background-image: url('http://localhost/phone_bg.png');
    background-size: 100%;
    background-repeat: no-repeat;
    .swiper_bg{
      position: absolute;
      top: 72px;
      left: 70px;
      width: 250px;
    }
    .swiper_p_1 {
      width: 150px;
      position: absolute;
      top: 120px;
      left: -15px;
      z-index: 3;
    }
    .swiper_p_2 {
      width: 154px;
      position: absolute;
      top: 128px;
      right: 2px;
      z-index: 3;
    }
    .swiper_p_3 {
      width: 450px;
      position: absolute;
      top: 280px;
      left: -34px;
      z-index: 3;
    }
    .swiper_p_4 {
          width: 411px;
    position: absolute;
    top: 380px;
    left: -15px;
    z-index: 3;
    }
  }
  .slider_right{
    position: absolute;
    left: 50%;
    top: 50%;
    margin-left: 80px;
    transform: translateY(-50%);
    h2{
      font-size: 24px;
      font-weight: bold;
      color: #333333;
    }
    p{
      font-size: 18px;
      margin-top: 20px;
      color: #333333;
      &+p{
        margin-top: 10px;
      }
    }
  }
  .swiper-container-vertical > .swiper-pagination-bullets{
    right: 30px;
  }
  .swiper-container-vertical > .swiper-pagination-bullets .swiper-pagination-bullet{
    margin: 10px 0;
  }
  .swiper-pagination-bullet-active{
    background: #5FE4B1;
  }
  .product{
    background: #F7F9FB;
    margin: auto;
    width: 100%;
    padding-bottom: 40px;
    overflow: hidden;
    position: relative;
    .content{
      width: 1180px;
      margin: auto;
      .title{
        font-size: 20px;
        color: #333;
        line-height: 20px;
        padding-top: 40px;
        padding-bottom: 30px;
        text-align: center;
      }
      .allitems{
        width: 1032px;
        margin: 0 auto;
        font-size: 0;
        .item{
          width: 384px;
          height: 360px;
          position: relative;
          display: inline-block;
          background-size: 100%;
          background-repeat: no-repeat;
          &.s_1{
            background-image: url('http://localhost/product_b1.jpg')
          }
          &.s_2{
            background-image: url('http://localhost/product_s1.jpg')
          }
          &.s_3{
            background-image: url('http://localhost/product_s1.jpg')
          }
          &.s_4{
            background-image: url('http://localhost/product_s1.jpg')
          }
          & + .item {
            margin-left: 24px;
            width: 192px;
          }
          .word{
            position: absolute;
            bottom: 15px;
            text-align: left;
            color: #fff;
            padding: 0 20px;
            h2{
              span{
                color: #f8f8f8;
                font-size: 20px;
                display: block;
              }
              .hr{
                width: 24px;
                height: 4px;
                background: #5FE4B1;
                margin-top: 20px;
                margin-bottom: 10px;
              }
              font-size: 24px;
              line-height: 28px;
            }
            p{
              padding-top: 10px;
              font-size: 14px;
              color: #f8f8f8;
              line-height: 22px;
            }
          }
        }
      }
    }
  }
  .server{
    margin: auto;
    width: 1032px;
    overflow: hidden;
    padding-bottom: 40px;
    .title{
      font-size: 20px;
      color: #333;
      line-height: 20px;
      padding-top: 40px;
      padding-bottom: 30px;
      text-align: center;
    }
    .server_inline {
      display: inline-block;
      float: left;
      width: 240px;
      text-align: left;
      & + .server_inline{
        margin-left: 24px;
      }
      img{
        width: 80px;
      }
      h2{
        font-size: 24px;
        margin-top: 18px;
      }
      p{
        font-size: 14px;
        color: #666666;
        margin-top: 20px;
        line-height: 26px;
      }
    }
  }
  .sym{
    height: 550px;
    background: url('http://localhost/sym.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    color: #fff;
    overflow: hidden;
    .content{
      width: 1180px;
      margin: 0 auto;
      position: relative;
      img{
        width: 50%;
        position: absolute;
        width: 50%;
        right: 0;
        top: -70px;
      }
    }
    .cont{
      width: 560px;
      margin: 118px 0 0 0;
      h3{
        font-size: 44px;
        margin-bottom: 50px;
      }
      p {
        font-size: 18px;
        line-height: 32px;
        margin: 0;
        padding: 0;
      }
      .hr{
        width: 88px;
        height: 4px;
        background: #fff;
        margin-top: 40px;
      }
    }
  }
</style>
