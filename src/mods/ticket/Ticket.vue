<template>
  <div class="station">
    <div class="in-bg"><yd-navbar title="票 务"></yd-navbar></div>
    <div>
      <yd-slider autoplay="3000">
        <yd-slider-item>
          <a href="#">
            <!--<img :src="carousel_1">-->
            <img src="http://static.ydcss.com/uploads/ydui/1.jpg">
          </a>
        </yd-slider-item>
        <yd-slider-item>
          <a href="#">
            <!--<img :src="carousel_2">-->
            <img src="http://static.ydcss.com/uploads/ydui/2.jpg">
          </a>
        </yd-slider-item>
        <yd-slider-item>
          <a href="#">
            <!--<img :src="carousel_3">-->
            <img src="http://static.ydcss.com/uploads/ydui/3.jpg">
          </a>
        </yd-slider-item>
      </yd-slider>
    </div>

    <div>
      <section class="aui-grid aui-margin-b-15">
        <div class="aui-row" >
          <div class="aui-col-xs-4" @click="goView('/ticket/ticket_info')">
            <!--<div class="aui-badge">88</div>-->
            <!--<i class="aui-iconfont aui-icon-home"></i>-->
            <div style="margin-top: 5px;margin-bottom: 5px"><i class="iconfont icon-ticket " style="opacity: 0.6"></i></div>
            <div class="aui-grid-label">车 票 信 息 </div>
          </div>
          <div class="aui-col-xs-4" @click="goView('/ticket/conductor')">
            <!--<i class="aui-iconfont aui-icon-gear"></i>-->
            <div style="margin-top: 5px;margin-bottom: 5px"><i class="iconfont icon-myline " style="opacity: 0.6"></i></div>
            <div class="aui-grid-label">按 售 票 员 查 询</div>
          </div>
          <div class="aui-col-xs-4" @click="goView('/ticket/reservedSeat_sell')">
            <!--<i class="aui-iconfont aui-icon-map"></i>-->
            <div style="margin-top: 5px;margin-bottom: 5px"><i class="iconfont icon-sorting " style="opacity: 0.6"></i></div>
            <div class="aui-grid-label">留 位 售 出</div>
          </div>

        </div>
      </section>
    </div>

    <footer class="aui-bar aui-bar-tab" id="footer">
      <div class="aui-bar-tab-item " tapmode @click="goView('/station/station')">
        <!--<i class="aui-iconfont aui-icon-home"></i>-->
        <div><i class="iconfont icon-homeline "></i></div>
        <div class="aui-bar-tab-label">站 务</div>
      </div>

      <div class="aui-bar-tab-item aui-active" tapmode @click="goView('/ticket/ticket')">
        <!--<i class="aui-iconfont aui-icon-star"></i>-->
        <div><i class="iconfont icon-ticket "></i></div>
        <div class="aui-bar-tab-label">票 务</div>
      </div>

      <div class="aui-bar-tab-item" tapmode @click="goView('/car/car')">
        <!--<i class="aui-iconfont aui-icon-cart"></i>-->
        <div><i class="iconfont icon-bus "></i></div>
        <div class="aui-bar-tab-label">车 方</div>
      </div>

      <div class="aui-bar-tab-item" tapmode @click="goView('/usermng/user')">
        <!--<i class="aui-iconfont aui-icon-my"></i>-->
        <div><i class="iconfont icon-myline "></i></div>
        <div class="aui-bar-tab-label">用 户</div>
      </div>
    </footer>

  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data() {
      return {
        carousel_1: 'static/1.jpg',
        carousel_2: 'static/2.jpg',
        carousel_3: 'static/3.jpg',
      }
    },
  }

</script>

