<template>
  <view class="content">
    <image class="logo" src="/static/logo.png"></image>
    <view>
      <text class="title">{{ title }}</text>
    </view>
    <uni-calendar :insert="true"></uni-calendar>
    <u-button>月落</u-button>
  </view>
</template>

<script>
import { uniCalendar } from "../../components/uni-calendar/uni-calendar.vue";
import { uButton } from "../../uview-ui/components/u-button/u-button.vue";
export default {
  components: {
    uniCalendar,
    uButton,
  },
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
};
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin: 200rpx auto 50rpx auto;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
