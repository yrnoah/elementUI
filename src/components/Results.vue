<template>
  <el-table
    :data="resultData"
    stripe
    style="width: 100%">
    <el-table-column prop="name" label="姓名" width="150"></el-table-column>
    <el-table-column prop="mobile" label="电话" width="150"></el-table-column>
    <el-table-column prop="price" label="价格" width="80"></el-table-column>
    <el-table-column prop="start" label="开始时间" width="180"></el-table-column>
    <el-table-column prop="end" label="结束时间" width="180"></el-table-column>
    <el-table-column prop="type" label="类型" width="80"></el-table-column>
    <el-table-column prop="location" label="地点"></el-table-column>
  </el-table>
</template>

<script>
  export default {
    props: ['resultData'],
    // data() {
    //   return {
    //     tableData: [{
    //       date: '2016-05-02',
    //       name: '王小虎',
    //       address: '上海市普陀区金沙江路 1518 弄'
    //     }, {
    //       date: '2016-05-04',
    //       name: '王小虎',
    //       address: '上海市普陀区金沙江路 1517 弄'
    //     }, {
    //       date: '2016-05-01',
    //       name: '王小虎',
    //       address: '上海市普陀区金沙江路 1519 弄'
    //     }, {
    //       date: '2016-05-03',
    //       name: '王小虎',
    //       address: '上海市普陀区金沙江路 1516 弄'
    //     }]
    //   }
    // },
    // mounted () {
    //   console.log(this);
    // }
  }
</script>