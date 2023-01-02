<template>
<div>
    <el-row>
      <el-col id='header-col1' :span="24">VT3D a visualization toolbox</el-col>
    </el-row>
    <hr>
    <h1>Developing Drosophila embryos and larvae atlas</h1>
    <el-row>
        <!-- card begin-->
        <el-col :span="8">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/E14.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                 <h2>E14-E16 embryo</h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button" @click.native="jumpE14" >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
        <!-- card begin-->
        <el-col :span="8">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/E16.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                 <h2>E16-E18 embryo</h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button"  @click.native="jumpE16" >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
        <!-- card begin-->
        <el-col :span="8">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/L1.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                 <h2>L1 larve</h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button"  @click.native="jumpL1" >Browse this data </el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
    </el-row>
    <el-row>
        <!-- card begin-->
        <el-col :span="12">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/L2.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                 <h2>L2 larva</h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button" @click.native="jumpL2"  >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
        <!-- card begin-->
        <el-col :span="12">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/L3.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                 <h2>L3 larva</h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button" @click.native="jumpL3"  >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
    </el-row>
    <hr>
    <el-row>
        <!-- card begin-->
        <el-col :span="12">
        <h1>Developing human heart atlas</h1>
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/heart.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button" @click.native="jumpHeart"  >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
        <!-- card begin-->
        <el-col :span="12">
        <h1>Preoptic hypothalamic atlas</h1>
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <img src="./assets/Hp.png" class="image">
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                <el-button type="text" style='font-weight:bold;font-size:22px;' class="button" @click.native="jumpHp"  >Browse this data</el-button>
              </el-col>
              <el-col :span="12">
                <el-button type="text" class="button" style='font-weight:bold;font-size:22px;'>Tutorial</el-button>
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
    </el-row>
    <el-footer>
        <div class='footer'>
            <p>For any inquiries about the website, please contact: guolidong@genomics.cn; liyao1@genomics.cn</p>
            <p>Powered by Element.js framework and Echarts.js library</p>
        </div>
    </el-footer>
</div>
</template>

<script>
export default {
    props: ['G_Atlas'],
    data() {
        return {
          currentSample: ''
        }
    },
    methods: {
      jumpE14(){
         window.location.href = '/vt3d_example/E14-16h/index.html?atlas=/vt3d_example/E14-16h';
      },
      jumpE16(){
         window.location.href = '/vt3d_example/E16-18h/index.html?atlas=/vt3d_example/E16-18h';
      },
      jumpL1(){
         window.location.href = '/vt3d_example/L1_a/index.html?atlas=/vt3d_example/L1_a';
      },
      jumpL2(){
         window.location.href = '/vt3d_example/L2_a/index.html?atlas=/vt3d_example/L2_a';
      },
      jumpL3(){
         window.location.href = '/vt3d_example/L3_b/index.html?atlas=/vt3d_example/L3_b';
      },
      jumpHeart(){
         window.location.href = '/vt3d_example/HumanHeart01/index.html?atlas=/vt3d_example/HumanHeart01';
      },
      jumpHp(){
         window.location.href = '/vt3d_example/hypo_preoptic/index.html?atlas=/vt3d_example/hypo_preoptic';
      },
    }
};
</script>

<style>
  #header-col1 {
    background-color: #4381e6;
    text-align: center;
    margin-top: 5px;
    margin-left: 5px;
    line-height: 100px;
    font-size: 50px;
    font-weight: bold;
    color: white;
  }
  .image {
    width: 100%;
    display: block;
  }
  .footer{
    background-color: white;
  }
  .card{
     border-width: 2px;
     border-style: solid;
     border-color:#111111;
     margin:10px
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
