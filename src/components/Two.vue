<template>
  <div id="two">
    <div id="cc"></div>
  </div>
</template>

<script>
export default {
name:"Two",
data() {
return {

}
},
methods:{
    fn(){
        var bb=this.$echarts.init(document.getElementById('cc'))
        var option = {
    xAxis: {
        type: 'category',
        data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
    },
    yAxis: {
        type: 'value'
    },
    series: [{
        data: [120, 200, 150, 80, 70, 110, 130],
        type: 'bar',
        showBackground: true,
        backgroundStyle: {
            color: 'rgba(220, 220, 220, 0.8)'
        }
    }]
};

            bb.setOption(option)
    }
},
//生命周期 - 创建完成（访问当前this实例）
created() {

},
//生命周期 - 挂载完成（访问DOM元素）
mounted() {
    this.fn()
}
}
</script>
<style scoped>
/* @import url(); 引入css类 */
#cc{
    width: 400px;
    height: 400px;
}
</style>