<!--
 * @Author       : xiaolin
 * @Date         : 2021-08-26 19:21:01
 * @LastEditors  : xiaolin
 * @LastEditTime : 2021-08-26 19:31:38
 * @Description  : 抽奖
 * @FilePath     : \lottery\src\components\lottery.vue
-->
<template>
  <div>
    <div>矿石：</div>
    <div>
      <LotteryItem />
      <LotteryItem />
      <LotteryItem />
      <LotteryItem />
      <LotteryItem />
    </div>
  </div>
</template>

<script>
import LotteryItem from "@/components/LotteryItem.vue";
export default {
  name: "Lottery",
  components: {
    LotteryItem,
  },
};
</script>

<style></style>
