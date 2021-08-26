<template>
  <div class="home is-flex">
    <div>
      <Module title="幸运抽奖">
        <Lottery />
      </Module>
    </div>
    <div>
      <Module title="抽奖纪录">
        <Record />
        <Record />
        <Record />
        <Record />
      </Module>
      <Module title="我的奖品">
        <Prize />
        <Prize />
        <Prize />
        <Prize />
        <Prize />
      </Module>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Module from "@/components/Module.vue";
import Lottery from "@/components/Lottery.vue";
import Record from "@/components/Record.vue";
import Prize from "@/components/Prize.vue";
export default {
  name: "Home",
  components: {
    Module,
    Lottery,
    Record,
    Prize,
  },
};
</script>

<style lang="scss">
.home {
  width: 1024px;
  margin: 0 auto;
}
</style>
