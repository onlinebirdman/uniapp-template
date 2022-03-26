<template>
  <swiper
    class="swiper"
    :indicator-dots="swiperConfig.indicatorDots"
    :autoplay="swiperConfig.autoplay"
    :interval="swiperConfig.interval"
    :duration="swiperConfig.duration"
  >
    <swiper-item>
      <view class="swiper-item uni-bg-red">
        A
      </view>
    </swiper-item>
    <swiper-item>
      <view class="swiper-item uni-bg-green">
        B
      </view>
    </swiper-item>
    <swiper-item>
      <view class="swiper-item uni-bg-blue">
        C
      </view>
    </swiper-item>
  </swiper>
</template>

<script setup lang="ts">
const swiperConfig = {
  indicatorDots: true,
  autoplay: true,
  interval: true,
  duration: 2000,
};
</script>

<style scoped lang="less">

</style>
