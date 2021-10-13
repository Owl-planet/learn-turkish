<template>
  <main>
    <div class="container">
      <div class="analysis">
        <apexchart class="apexchart-area" width="340" type="bar" :options="chartOptions" :series="series"></apexchart>
      </div>
      <div class="row-1 progress">
        <a href="#">
          <h3>MY PROGRESS</h3>
        </a>
        <i class="fa fa-archive" aria-hidden="true"></i>
        <p>0</p>
        <h2>Total words</h2>
      </div>
      <div class="row-2 progress">
        <a href="#">
          <h3>All stats</h3>
        </a>
        <i class="fa fa-eye" aria-hidden="true"></i>
        <p>0</p>
        <h2>Words at risk</h2>
      </div>
      <div class="row-3 progress-2">
        <a href="#">
          <h3>CURRENTLY LEARNING</h3>
        </a>
        <h3>Change</h3>
        <h4>0 active deck</h4>
        <i class="fa fa-flask" aria-hidden="true"></i>
        <h2>Next Level Turkish</h2>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  data: function() {
    return {
      chartOptions: {
        chart: {
          id: "vuechart-example",
        },
        xaxis: {
          categories: ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
        },
      },
      series: [
        {
          name: "series-1",
          data: [0, 0, 0, 0, 0, 0, 0, 0],
        },
      ],
    };
  },
};
</script>
