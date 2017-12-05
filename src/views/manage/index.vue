<template>
    <div class='manage'>
        <header-top></header-top>
        <div class="manage-box">
            <slider></slider>
        </div>
    </div>
</template>

<script>
  import HeaderTop from '@/components/Header'
  import Slider from '@/components/Slider'

  export default {
    components: {
      HeaderTop,
      Slider
    },
    data () {
      return {}
    },
    computed: {},
    methods: {},
    created () {
    }
  }
</script>

<style lang="less" scoped>
    .manage{
        width: 100%;
        height: 100%;
        &-box{
            padding-top: 80px;
        }
    }
</style>
