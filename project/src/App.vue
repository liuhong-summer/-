<template>
  <div >
    <el-container>
      <el-header class="header">
        <el-row>
          <el-col :span="8">
            <i class="el-icon-location color-blue font-size-18"></i><span>{{position}}</span>
          </el-col>
          <el-col :span="8">
            <i class="el-icon-tickets color-blue font-size-18"></i>
            {{subject}}</el-col>
          <el-col :span="8">
            {{score}}</el-col>
        </el-row>
      </el-header>
      <el-main>
        <el-row>
          <el-col :span="12" class="width-45">
            <div class="grid-content bg-blue position-relative">
              <img src="../static/images/vip.png" alt="" class="vip">
              <img src="../static/images/search_1.png" alt="" class="display-inline-block img">
              <div class="display-inline-block content-img">
                <p>我能上的学校</p>
                <p><span class="font-size-18">{{mySchoolNum}}</span>所</p>
              </div>
            </div>
          </el-col>
          <el-col :span="12" class="width-45">
            <div class="grid-content bg-orange position-relative">
              <img src="../static/images/vip.png" alt="" class="vip">
              <img src="../static/images/search1.png" alt="" class="display-inline-block img">
              <div class="display-inline-block content-img">
                <p>我能上的专业</p>
                <p><span class="font-size-18">{{myProjectNum}}</span>所</p>
              </div>
            </div>
          </el-col>
        </el-row>
      </el-main>
    </el-container>
  </div>
</template>
<script>
export default {
  data () {
    return {
      position: '四川',
      subject: '文科',
      score: '586',
      mySchoolNum: '433',
      myProjectNum: '333'
    };
  }};
</script>
<style>
  .header{
    height: 50px;
    line-height: 50px;
  }
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
  /**/
  .el-main{
    padding: 0;
  }
  .el-main .el-row{
    display: flex;
    justify-content: space-between;
  }
  .el-row .width-45{
    width: 45%;
  }
  .img{
    width: 35%;
    vertical-align: middle;
    color: white;
    padding: 10px 1% 10px 5%;
  }
  .content-img{
    width: 53%;
    padding-right: 2%;
    text-align: right;
    vertical-align: middle;
    color: white;
    font-size: 1.2rem;
  }
  .vip{
    width: 18%;
    position: absolute;
    left: -2%;
    top: -5%;
  }
</style>
