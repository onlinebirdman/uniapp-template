<template>
  <swiper
    class="swiper"
    :indicator-dots="swiperConfig.indicatorDots"
    :autoplay="swiperConfig.autoplay"
    :interval="swiperConfig.interval"
    :duration="swiperConfig.duration"
    :circular="swiperConfig.circular"
  >
    <swiper-item
      v-for="(banner, index) in props.list"
      :key="index"
    >
      <view class="swiper-item uni-bg-red">
        <image
          class
          :src="banner"
          mode="widthFix"
        />
      </view>
    </swiper-item>
  </swiper>
</template>

<script setup lang="ts">

const props = withDefaults(defineProps<{
  list: string[]
  size: number[]
}>(), {
  list: [],
  size: []
})

// const props = defineProps({
//   list: {
//     type: Array,
//     required: true,
//     default: () => [],
//   },
// });

const swiperConfig = {
  indicatorDots: true,
  autoplay: true,
  duration: 500,
  circular: true,
  interval: 2000,
};
</script>

<style scoped lang="less">
</style>
