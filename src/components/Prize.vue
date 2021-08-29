<!--
 * @Author       : xiaolin
 * @Date         : 2021-08-26 19:36:18
 * @LastEditors  : xiaolin
 * @LastEditTime : 2021-08-26 19:38:39
 * @Description  : 奖品
 * @FilePath     : \lottery\src\components\Prize.vue
-->
<template>
  <div class="prize">
    <div class="btn-left">
      <i class="icon"> </i>
    </div>
    <lottery-item v-for="item in priceInfo" :key="item.id" v-bind="item">
    </lottery-item>
    <div class="btn-right">
      <i class="icon"> </i>
    </div>
  </div>
</template>

<script>
import img1 from "@/assets/img/assets_1.png";
import img2 from "@/assets/img/assets_2.png";
import img3 from "@/assets/img/assets_3.png";
import LotteryItem from "@/components/LotteryItem";

export default {
  name: "Prize",
  components: {
    LotteryItem,
  },
  data() {
    return {
      priceInfo: [],
    };
  },
  methods: {
    fetchPriceInfo() {
      this.priceInfo = [
        {
          src: img1,
          describe: "杯子",
          id: 1,
        },
        {
          src: img2,
          describe: "switch",
          id: 2,
        },
        {
          src: img3,
          describe: "t恤",
          id: 3,
        },
      ];
    },
  },
  created() {
    this.fetchPriceInfo();
  },
};
</script>

<style lang="scss">
.prize {
  margin-right: 1em;
  display: flex;
}
</style>
