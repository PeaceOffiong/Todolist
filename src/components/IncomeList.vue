<template>
  <div class="income-list">
    <Incomeitems
      v-for="data in state.income"
      :key="data.id"
      :income="data"
      :state="state"
    />
  </div>
</template>

<script>
import Incomeitems from "./Incomeitem";

export default {
  props: {
    state: Object,
  },
  setup() {
    return {
      Incomeitems,
    };
  },
};
</script>

<style scoped>
.income-list {
  margin-top: 30px;
  padding: 15px;
}
</style>