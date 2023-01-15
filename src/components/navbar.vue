<template>
  <header>
    <h1>Income Tracker</h1>
    <div class="total-income">N{{ totalIncome }}</div>
  </header>
</template>

<script>
export default {
  props: {
    totalIncome: Number,
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  background-color: #313131;
  border-bottom: 5px solid #FFCE00;
}

header h1 {
  color: #EEE;
  font-size: 20px;
}

header .total-income {
  font-family: sanserif;
  background-color: #FFCE00;
  color: #fff;
  font-size: 20px;
  font-weight: 900;
  padding: 5px 10px;
  min-width: 100px;
  text-align: center;
  border-radius: 8px;
  box-shadow: inset 0px 0px 6px rgba(0, 0, 0, 0.25);
  text-shadow: 0px 3px 3px rgba(0, 0, 0, 0.25);
}
</style>