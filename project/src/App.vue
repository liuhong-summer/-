<template>
  <div >
    <div class="contain">
      <el-row :gutter="20">
        <el-col :span="8">
          <i class="el-icon-location color-blue font-size-18"></i><span>{{position}}</span>
        </el-col>
        <el-col :span="8">{{subject}}</el-col>
        <el-col :span="8">{{score}}</el-col>
      </el-row>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      position: '四川',
      subject: '文科',
      score: '586'
    };
  }};
</script>
<style>
  .el-row {
    margin-bottom: 20px;
  }
  .el-row:last-child{
    margin-bottom: 0;
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .contain .el-row{
    text-align: center;
  }
</style>
