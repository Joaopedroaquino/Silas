<template>
  <div>
    <client-only>
      <apexchart
        type="donut"
        width="480px"
        :options="chartOptions"
        :series="series"
      ></apexchart>
    </client-only>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'nuxt-property-decorator'

@Component({})
export default class GraphicFeedbackComponent extends Vue {
  series = [44, 55, 41, 17, 15]
  chartOptions = {
    labels: ['Apple', 'Mango', 'Orange', 'Watermelon'],
  }
  //   chartOptions: ({
  //     chart: {
  //       width: 380,
  //       type: 'pie',
  //     },
  //     labels: [
  //       'FEEDBACKS PROGRAMADOS',
  //       'FEEDBACKS CONCLUÍDOS',
  //       'FEEDBACKS PENDENTES',
  //       'FEEDBACKS ATRASADOS',
  //     ],
  //     colors: ['#3fa3ad', '#459d5c', '#e3893e', '#b54444'],
  //     responsive: [
  //       {
  //         breakpoint: 480,
  //         options: {
  //           chart: {
  //             width: '250px',
  //           },
  //           legend: {
  //             position: 'bottom',
  //           },
  //         },
  //       },
  //     ],
  //   }),
}
</script>

<style></style>
