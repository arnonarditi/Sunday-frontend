<template>
  <section class="flex flex-col align-center chart-container">
    <h3 class="chart-head">Tasks by members</h3>
    <BarChart class="chart inner-bar-chart" :chartData="data" :options="options" />
  </section>
</template>

<script>
import { BarChart } from "vue-chart-3";
import { Chart, registerables } from "chart.js";

Chart.register(...registerables);

export default {
  name: "Home",
  props: {
    data: Object,
    options: Object,
  },
  data() {
    return {

    };
  },
  mounted() {
  },
  components: {
    BarChart,
  },
};
</script>