<template>
<div>
    <header>
        <el-row id='header-row'>
          <el-col id='header-col1' :span="6">VT3D</el-col>
          <el-col id='header-col2' :span="6"><img ></el-col>
          <el-col id='header-col3' :span="6">
            <el-button style='font-weight:bold;color:#8b8c8f;font-size:22px;background-color:white;border-style:none;' type="primary" icon='el-icon-info' @click='jumpIntro'>About US</el-button>
            </el-col>
        </el-row>
    </header>


    <el-container>
        <el-main>
        <div id='canvas'>
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
        </div>
        </el-main>
       
        <el-footer>
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
      },
      jumpIntro(){
        console.log('about us');
      }
    }
};
</script>

<style>
  #header-row{
    margin: 0 auto;
    width: 100%;
    position: relative;
  }
  #header-col1 {
    background-color: #4381e6;
    width: 200px;
    text-align: center;
    margin-top: 5px;
    margin-left: 5px;
    line-height: 100px;
    font-size: 50px;
    font-weight: bold;
    color: white;
  }
  #header-col2 {
    margin-left: 20px;
    width:50%;
  }
  #header-col3 {
    width: 120px;
    line-height: 100px;
    margin-right: 0%;
    min-height: 50px;
  }

  #canvas {
    max-width: 2000px;
    justify-content: center;
  }
  .el-main {
    margin-top: 15px;
    margin-bottom: 15px;
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
    position: relative;
  }
  body > .el-container {
    margin-bottom: 100px;
  }
  

  .el-row {
    margin-bottom: 20px;
    margin-left: 40%;
    display: flex;
    flex-wrap: wrap;
  }
  .el-row:last-child {
    margin-bottom: 0;
  }
  .el-col {
    border-radius: 10px;
    z-index: 999;
    float: left;
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
    background-color: white;
  }
  .el-footer {
    background-color: white;
    color: #8b8c8f;
    font-size: 14px;
    text-align: center;
    margin-top: 20px;
    width: 100%;
  }
</style>
