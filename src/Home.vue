<template>
<div>
    <el-row>
      <el-col id='header-col1' :span="24">VT3D a visualization toolbox for 3D transcriptomic data</el-col>
    </el-row>
    <hr>
    <el-row>
      <el-col :span="18"> 
        <h1>Developing Drosophila embryos and larvae atlas</h1>
      </el-col>
      <el-col :span="6"> 
        <h1><a href="https://doi.org/10.1016/j.devcel.2022.04.006" target="_blank"> Reference </a></h1>
      </el-col>
    </el-row>
    <el-row>
        <!-- card begin-->
        <el-col :span="8">
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <div @click="jumpE14" >
                    <img src="./assets/E14.png" class="image" >
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                 <h2>E14-E16 embryo</h2>
              </el-col>
              <el-col :span="12">
                <h2><a href="/vt3d_example/E14-16h/index.html?atlas=/vt3d_example/E14-16h" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
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
                <div @click="jumpE16" >
                  <img src="./assets/E16.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                 <h2>E16-E18 embryo</h2>
              </el-col>
              <el-col :span="12">
                <h2><a href="/vt3d_example/E16-18h/index.html?atlas=/vt3d_example/E16-18h" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item  title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
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
                <div @click="jumpL1" >
                  <img src="./assets/L1.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                 <h2>L1 larve</h2>
              </el-col>
              <el-col :span="12">
                <h2><a href="/vt3d_example/L1_a/index.html?atlas=/vt3d_example/L1_a" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
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
                <div @click="jumpL2" >
                  <img src="./assets/L2.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                 <h2>L2 larva</h2>
              </el-col>
              <el-col :span="12">
                <h2><a href="/vt3d_example/L2_a/index.html?atlas=/vt3d_example/L2_a" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
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
                <div @click="jumpL3" >
                   <img src="./assets/L3.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="12">
                 <h2>L3 larva</h2>
              </el-col>
              <el-col :span="12">
                <h2><a href="/vt3d_example/L3_b/index.html?atlas=/vt3d_example/L3_b" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
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
           <el-row>
              <el-col :span="18"> 
                <h1>Developing human heart atlas</h1>
              </el-col>
              <el-col :span="6"> 
                <h1><a href="https://doi.org/10.1016/j.cell.2019.11.025" target="_blank"> Reference </a></h1>
              </el-col>
           </el-row>
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <div @click="jumpHeart" >
                   <img src="./assets/heart.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <h2><a href="/vt3d_example/HumanHeart01/index.html?atlas=/vt3d_example/HumanHeart01" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
        <!-- card begin-->
        <el-col :span="12">
           <el-row>
              <el-col :span="18"> 
                <h1>Preoptic hypothalamic atlas</h1>
              </el-col>
              <el-col :span="6"> 
                <h1><a href="http://dx.doi.org/10.1126/science.aau5324" target="_blank"> Reference </a></h1>
              </el-col>
           </el-row>
          <div class='card'>
           <el-row>
              <el-col :span="24">
                <div @click="jumpHp" >
                <img src="./assets/Hp.png" class="image">
                </div>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <h2><a href="/vt3d_example/hypo_preoptic/index.html?atlas=/vt3d_example/hypo_preoptic" target="_blank"> Browse this data </a></h2>
              </el-col>
           </el-row>
           <el-row>
              <el-col :span="24">
                <el-collapse>
                    <el-collapse-item   title="Tutorial" name="1">
                      <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
                      <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
                    </el-collapse-item>
                </el-collapse  >
              </el-col>
           </el-row>
          </div>
        </el-col>
        <!-- card end-->
    </el-row>
    <hr>
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
         window.open('/vt3d_example/E14-16h/index.html?atlas=/vt3d_example/E14-16h','_blank');
      },
      jumpE16(){
         window.open('/vt3d_example/E16-18h/index.html?atlas=/vt3d_example/E16-18h','_blank');
      },
      jumpL1(){
         window.open('/vt3d_example/L1_a/index.html?atlas=/vt3d_example/L1_a','_blank');
      },
      jumpL2(){
         window.open('/vt3d_example/L2_a/index.html?atlas=/vt3d_example/L2_a','_blank');
      },
      jumpL3(){
         window.open('/vt3d_example/L3_b/index.html?atlas=/vt3d_example/L3_b','_blank');
      },
      jumpHeart(){
         window.open('/vt3d_example/HumanHeart01/index.html?atlas=/vt3d_example/HumanHeart01','_blank');
      },
      jumpHp(){
         window.open('/vt3d_example/hypo_preoptic/index.html?atlas=/vt3d_example/hypo_preoptic','_blank');
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
