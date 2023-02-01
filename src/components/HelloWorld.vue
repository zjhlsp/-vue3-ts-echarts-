<template>
  <div class="main">
    <myEchart 
    type="Pie"
    :data="pieData"
    :option="{title: '菜品售出统计'}"
    />
  </div>
</template>
<script setup lang='ts'>
import myEchart from './myEcharts/MyEchart.vue';
import { reactive } from 'vue';


const pieData = reactive({
  seriesName: '菜品统计',
  seriesData: [
    { value: 730, name: '小炒肉' },
    { value: 210, name: '番茄炒鸡蛋' },
    { value: 330, name: '清蒸鲈鱼' },
    { value: 530, name: '小龙虾' },
    { value: 600, name: '蒜蓉青菜' }
]
})
</script>
<style lang='css' scoped>
</style>