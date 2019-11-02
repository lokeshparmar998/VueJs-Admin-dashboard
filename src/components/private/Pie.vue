<template>
   <div class="box">
      <h3>Top Categories</h3>
      <div ref="chartdiv" class="just"></div>
     <!-- <div class="container-flex">
            <div class="row">
                <div class="col-md-6" ref="chartdiv" style="background-color:#FFFFFF;border: 0.15px solid lightgray;">
                </div>
            </div>
        </div> -->
   </div>
</template>
<script>
import * as am4core from "@amcharts/amcharts4/core";
import * as am4charts from "@amcharts/amcharts4/charts";
import am4themes_animated from "@amcharts/amcharts4/themes/animated";

am4core.useTheme(am4themes_animated);
export default {
    mounted(){
       let chart = am4core.create(this.$refs.chartdiv, am4charts.PieChart);
       chart.data = [{
  "country": "Lithuania",
  "litres": 501.9
}, {
  "country": "Czech Republic",
  "litres": 301.9
}, {
  "country": "Ireland",
  "litres": 201.1
}, {
  "country": "Germany",
  "litres": 165.8
}, {
  "country": "Australia",
  "litres": 139.9
}, {
  "country": "Austria",
  "litres": 128.3
}, {
  "country": "UK",
  "litres": 99
}, {
  "country": "Belgium",
  "litres": 60
}, {
  "country": "The Netherlands",
  "litres": 50
}];

// Add and configure Series

var pieSeries = chart.series.push(new am4charts.PieSeries());
//pieChart.radius = am4core.percent.percent(50);
pieSeries.dataFields.value = "litres";
pieSeries.labels.template.disabled = true;
pieSeries.ticks.template.disabled = true;
pieSeries.dataFields.category = "country";

pieSeries.radius.value=200;
//chart.legend = new am4charts.Legend();
    },
    beforeDestroy() {
    if (this.chart) {
      this.chart.dispose();
    }
  }
}
</script>
<style scoped>
   .box{
    text-align: center;
    border: 0.15px solid lightgray;
    margin-left: 60px;
    position: relative;
    height: 300px;
    width: 88%
   }
</style>