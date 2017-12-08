<template>
  <div id="app">
      <div class="banner">
          <ul class="pic">
              <li><a href="javascript:;"><img src="images/DSC01627.jpg" alt="pic1"></a></li>
              <li><a href="javascript:;"><img src="images/DSC01628.jpg" alt="pic2"></a></li>
              <li><a href="javascript:;"><img src="images/DSC02637.jpg" alt="pic3"></a></li>
              <li><a href="javascript:;"><img src="images/DSC01627.jpg" alt="pic1"></a></li>
          </ul>
      </div>
      <div class="links">
          <ul class="links-items">
              <!--<li class="links-item" @click="getMore">-->
                  <!--<span>全部银行</span>-->
                  <!--<span :class="down ? 'dropdown' : 'dropup'"></span>-->
              <!--</li>-->
              <!--<li class="links-item">-->
                  <!--<span>全部用途</span>-->
                  <!--<span class="dropdown"></span>-->
              <!--</li>-->
              <!--<li class="links-item">-->
                  <!--<span>全部等级</span>-->
                  <!--<span class="dropup"></span>-->
              <!--</li>-->
              <li class="links-item" v-for="(item, index) in links" :key="index">
                  <span>{{item}}</span>
                  <span :class="down ? 'dropdown' : 'dropup'"></span>
              </li>
          </ul>
      </div>
      <div class="item-detail">
          <div class="item-detail-lists">
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
              <p>000</p>
          </div>
          <div class="item-detail-model">

          </div>
      </div>
      <div class="cards">
          <ul class="cards-items">
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>免费道路救援服务</li>
                          <li>信用卡积分换车险某某</li>
                      </ul>
                      <p class="card-btn">
                          <a href="javascript:;">年轻白领时尚必备</a><a href="javascript:;">年轻白领时尚必备</a>
                      </p>
                  </div>
              </li>
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>免费道路救援服务</li>
                          <li>信用卡积分换车险某某</li>
                      </ul>
                      <p class="card-btn">
                          <a href="javascript:;">年轻白领时尚必备</a><a href="javascript:;">年轻白领时尚必备</a>
                      </p>
                  </div>
              </li>
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>免费道路救援服务</li>
                          <li>信用卡积分换车险某某</li>
                      </ul>
                      <p class="card-btn">
                          <a href="javascript:;">年轻白领时尚必备</a><a href="javascript:;">年轻白领时尚必备</a>
                      </p>
                  </div>
              </li>
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>信用卡积分换车险某某</li>
                      </ul>
                      <p class="card-btn">
                          <a href="javascript:;">年轻白领时尚必备</a><a href="javascript:;">年轻白领时尚必备</a>
                      </p>
                  </div>
              </li>
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>免费道路救援服务</li>
                          <li>信用卡积分换车险某某</li>
                      </ul>
                  </div>
              </li>
              <li class="cards-item">
                  <div class="cards-item-left">
                      <img src="" alt="加载中..."/>
                  </div>
                  <div class="cards-item-right">
                      <p class="card-names">
                          <span class="card-name">平安车主卡</span>
                          <a href="javascript:;" class="card-application">立即申请</a>
                      </p>
                      <ul class="card-links">
                          <li>免费道路救援服务</li>
                          <li>信用卡积分换车险某某</li>
                      </ul>
                      <p class="card-btn">
                          <a href="javascript:;">年轻白领时尚必备</a><a href="javascript:;">年轻白领时尚必备</a>
                      </p>
                  </div>
              </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      down: true,
      links: ['全部银行', '全部用途', '全部等级']
    }
  },
  methods: {
    getMore () {
      this.down = !this.down
    }
  }
}
</script>

<style lang="less">
    #app{
        position: relative;
        width: 100%;
        height: 100%;
        .banner{
            position: relative;
            width: 100%;
            height: 120px;
            overflow: hidden;
            .pic{
                width:400%;
                height: 120px;
                position: absolute;
                left:0;
                animation: focusmap 12s infinite;
                li{
                    float: left;
                    width: 25%;
                    height: 120px;
                    background: #099;
                    img {
                        width: 25%;
                        height: 120px;
                    }
                }
            }
            @keyframes focusmap {
                0%,30%{
                    left: 0;
                }
                35%,65%{
                    left: -100%;
                }
                70%,99%{
                    left: -200%;
                }
                100%{
                    left: -300%;
                }

            }
        }
        .links{
            width: 100%;
            height: 48px;
            border-bottom: 1px solid rgba(0,0,0,0.08);
            &-items{
                width: 100%;
                height: 100%;
                display: flex;
                align-items: center;
            }
            &-item{
                flex: 1;
                font-size: 15px;
                color: rgba(0,0,0,0.87);
                height: 26px;
                line-height: 26px;
                text-align: center;
                border-right: 1px solid rgba(0,0,0,0.12);
                &:last-child{
                    border: 0;
                }
                span{
                    margin-left: 10px;
                    display: inline-block;
                    height: 26px;
                    vertical-align: middle;
                }
                .dropdown{
                    width: 24px;
                    height: 24px;
                    background: url("./../static/images/arrow_dropdown@3x.png") center no-repeat;
                    background-size: cover;
                }
                .dropup{
                    width: 24px;
                    height: 24px;
                    background: url("./../static/images/arrow_dropup@3x.png") center no-repeat;
                    background-size: cover;
                }
            }
        }
        .item-detail{
            position: absolute;
            width: 100%;
            height: 80vh;
            overflow: hidden;
            z-index: 100;
            &-lists{
                background-color: #fff;
                width: 100%;
                height: 50vh;
                overflow: hidden;
                overflow-y: auto;
            }
            &-model{
                position: fixed;
                left: 0;
                bottom: 0;
                width: 100%;
                height: 30vh;
                background: rgba(0,0,0,0.38);
            }
        }
        .cards{
            width: 100%;
            &-items{
            }
            &-item{
                display: flex;
                align-items: center;
                height: 115px;
                margin: 0 16px;
                border-bottom: 1px solid rgba(0,0,0,0.08);
                &:last-child{
                    border: 0;
                }
                &-left{
                    width: 109px;
                    height: 69px;
                    background: #D8D8D8;
                    border-radius: 4px;
                    img{
                        width: 100%;
                        height: 100%;
                    }
                }
                &-right{
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    flex: 1;
                    margin-left: 13px;
                }
                .card-names{
                    margin-top: -5px;
                    display: flex;
                    justify-content: space-between;
                    .card-name{
                        font-size: 15px;
                        color: rgba(0,0,0,0.87);
                        line-height: 23px;
                    }
                    .card-application{
                        display: inline-block;
                        width: 64px;
                        height: 24px;
                        line-height: 24px;
                        text-align: center;
                        background: #FF5722;
                        border-radius: 2px;
                        font-size: 13px;
                        color: #FFFFFF;
                    }
                }
                .card-links{
                    font-size: 13px;
                    color: rgba(0,0,0,0.54);
                    line-height: 20px;
                }
                .card-btn{
                    margin-top: 3px;
                    a{
                        display: inline-block;
                        height: 17px;
                        line-height: 17px;
                        padding: 0 3px;
                        margin-right: 5px;
                        border: 1px solid #5C6BC0;
                        border-radius: 2px;
                        font-size: 10px;
                        color: #5C6BC0;
                    }
                }
            }
        }
    }
</style>
