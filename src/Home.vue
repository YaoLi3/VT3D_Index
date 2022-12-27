<template>
<div>
<el-container>
  <el-header>VT3D</el-header>
  <el-main>
        <el-row :gutter="20">
            <el-col :span="6"><div class="grid-content bg-purple">test1</div></el-col>
            <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
        </el-row>
        <el-row :gutter="20">
            <el-col :span="6"><div class="grid-content bg-purple">test1</div></el-col>
            <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
        </el-row>
        <el-row :gutter="20">
            <el-col :span="6"><div class="grid-content bg-purple">test1</div></el-col>
            <el-col :span="6"><div class="grid-content bg-purple"></div></el-col>
        </el-row>
  </el-main>
  <el-footer style='font-size: 12px'>
    <el-row>
      <el-col><div class='footer'>
        <p>For any inquiries about the website, please contact: guolidong@genomics.cn; liyao1@genomics.cn</p>
      </div></el-col>
      <el-col><div class='footer'>
        <p>Powered by Element.js framework and Echarts.js library.</p>
      </div></el-col>
    </el-row>
  </el-footer>
</el-container>
</div>
</template>

<script>
export default {
    props: ['G_Atlas'],
    data() {
        return {}
    },
    methods: {
      switchSample(){
        // jump to a new web
      }
    }
};
</script>

<style>
  .el-header {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
  .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
  }
  body > .el-container {
    margin-bottom: 100px;
  }
  .el-row {
    margin-bottom: 60px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 10px;
    z-index: 999;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 100px;
  }
  .row-bg {
    padding: 50px 50px;
    background-color: #f9fafc;
  }
  .footer{
    background-color: #B3C0D1;
  }
</style>
