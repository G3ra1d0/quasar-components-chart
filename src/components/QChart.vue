<template>
  <canvas :id="identifier" :style="stilo"></canvas>
</template>

<script>
import Chart from "chart.js";

export default {
  name: "QChart",
  props: ["identifier", "stilo", "type", "labels", "datasets", "options"],
  data() {
    return {};
  },
  mounted() {
    let ctx = document.getElementById(this.identifier);
    new Chart(ctx, {
      type: this.type,
      data: {
        labels: this.labels,
        datasets: this.datasets
      },
      options: this.options
    });
  }
};
</script>
