<template>
<div>
    <el-container>
        <el-header>
            VT3D
        </el-header>
        
        <el-main>
            <el-row :gutter="20">
                <el-col :span="6"><div class="grid-content bg-purple">
                    test1
                </div></el-col>
                <el-col :span="6"><div class="grid-content bg-purple">
                    <a href="/vt3d_example/E16-18h/index.html?atlas=/vt3d_example/E16-18h" target="_blank">E16-18h</a > 
                </div></el-col>
            </el-row>
            <el-row :gutter="20">
                <el-col :span="6"><div class="grid-content bg-purple">
                    test1
                </div></el-col>
                <el-col :span="6"><div class="grid-content bg-purple">
                    <a href="/vt3d_example/L1_a/index.html?atlas=/vt3d_example/L1_a" target="_blank">L1_a</a > 
                </div></el-col>
            </el-row>
            <el-row :gutter="20">
                <el-col :span="6"><div class="grid-content bg-purple">
                    <a href="/vt3d_example/L3_b/index.html?atlas=/vt3d_example/L3_b" target="_blank">L3_b</a > 
                </div></el-col>
                <el-col :span="6"><div class="grid-content bg-purple">
                    <a href="/vt3d_example/L2_a/index.html?atlas=/vt3d_example/L2_a" target="_blank">L2_a</a > 
                </div></el-col>
            </el-row>
        </el-main>
       
        <el-footer style='font-size: 12px'>
            <div class='footer'>
                <p>For any inquiries about the website, please contact: guolidong@genomics.cn; liyao1@genomics.cn</p>
                <p>Powered by Element.js framework and Echarts.js library</p>
            </div>
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
    background-color: #e9fa2d;
    color: #333;
    text-align: center;
    line-height: 60px;
    width: 100%;
    height: 50%;
    position: relative;
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
    position: relative;
  }
  .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    margin: 0 auto;
    width: 100%;
  }
  body > .el-container {
    margin-bottom: 100px;
  }
  .el-row {
    margin-bottom: 60px;
    margin-left: 40%;
    display: flex;
    flex-wrap: wrap;
  }
  .el-col {
    border-radius: 10px;
    z-index: 999;
    margin-left: 15%;
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
