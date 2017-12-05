<template>
    <div class='header'>
        <div class="header-title">
            <span>后台管理系统</span>
        </div>
        <div class="header-user">
            <span @mouseover="showMore = true" @mouseout="showMore = false">管理员</span>
            <ul class="header-user-more" :class="showMore ? 'on' : 'hide'" @mouseover="showMore = true" @mouseout="showMore = false">
                <li>首页</li>
                <li>退出</li>
                <div class="more-arrow"></div>
            </ul>
        </div>
    </div>
</template>

<script>
  export default {
    components: {},
    data () {
      return {
        showMore: false
      }
    },
    computed: {},
    methods: {
//      LoadMore () {}
    },
    created () {
    }
  }
</script>

<style lang="less" scoped>
    .header{
        background-color: #22D0B2;
        width: 100%;
        height: 80px;
        line-height: 80px;
        color: #fff;
        &-title {
            float: left;
            margin-left: 20px;
        }
        &-user{
            position: relative;
            float: right;
            margin-right: 80px;
            cursor: pointer;
            span{
                display: inline-block;
            }
            &-more{
                position: absolute;
                top: 60px;
                left: -20px;
                line-height: 2;
                padding: 10px 0;
                background-color: #fff;
                font-size: 14px;
                color: #5a5e66;
                font-weight: inherit;
                text-align: center;
                width: 100px;
                border-radius: 5px;
                border: 1px solid #e6ebf5;
                box-shadow: 0 2px 12px 0 rgba(0,0,0,.1);
                .more-arrow{
                    position: absolute;
                    top: -6px;
                    left: 50px;
                    &:after{
                        content: " ";
                        position: absolute;
                        border-color: transparent;
                        border-style: solid;
                        border-width: 6px;
                        top: 1px;
                        margin-left: -6px;
                        border-top-width: 0;
                        border-bottom-color: #fff;
                    }
                }
                li{
                    line-height: 28px;
                }
                li:hover{
                    cursor: pointer;
                    background-color: #ecf5ff;
                    color: #409EFF;
                }
            }
            .hide{
                display: none;
            }
            .on{
                display: block;
            }
        }
    }
</style>
