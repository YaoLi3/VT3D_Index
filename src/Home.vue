<template>
<div class='background'>
<div class='center-div'>
    <el-row id='header-col1' >
      <el-col  :span="24"><h1>VT3D&#58; a visualization toolbox for 3D transcriptomic data</h1></el-col>
    </el-row>
    <hr>
    <el-tabs v-model="activeName" type="border-card" >
      <el-tab-pane label="Atlases" name="atlas">
        <el-row>
          <el-col :span="18"> 
            <el-row>
              <el-col :span="24"> 
                <h2>Developing <i>Drosophila</i> embryos and larvae</h2>
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
                         <h3>E14-16h embryo</h3>
                      </el-col>
                      <el-col :span="12">
                        <h3><a href="/vt3d_example/E14-16h/index.html?atlas=/vt3d_example/E14-16h" target="_blank"> Browse</a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; 14h-16h embryo of <i>drosophila</i><br>
                                  number of slices&#58; 13<br>
                                  number of bins&#58; 15,295<br>
                                  number of genes&#58; 13,668<br>
                                  number of models&#58; 11 </p>
                              </div>
                            </el-collapse-item>
                        </el-collapse>
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
                         <h3>E16-18h embryo</h3>
                      </el-col>
                      <el-col :span="12">
                        <h3><a href="/vt3d_example/E16-18h/index.html?atlas=/vt3d_example/E16-18h" target="_blank"> Browse </a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; 16h-18h embryo of <i>drosophila</i><br>
                                  number of slices&#58; 11<br>
                                  number of bins&#58; 14,634<br>
                                  number of genes&#58; 12,850<br>
                                  number of models&#58; 11 </p>
                              </div>
                            </el-collapse-item>
                        </el-collapse>
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
                         <h3>L1 larva</h3>
                      </el-col>
                      <el-col :span="12">
                        <h3><a href="/vt3d_example/L1_a/index.html?atlas=/vt3d_example/L1_a" target="_blank"> Browse  </a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; L1 larva of <i>drosophila</i><br>
                                  number of slices&#58; 20<br>
                                  number of bins&#58; 17,787<br>
                                  number of genes&#58; 13,803<br>
                                  number of models&#58; 10 </p>
                              </div>
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
                         <h3>L2 larva</h3>
                      </el-col>
                      <el-col :span="12">
                        <h3><a href="/vt3d_example/L2_a/index.html?atlas=/vt3d_example/L2_a" target="_blank"> Browse </a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; L2 larva of <i>drosophila</i><br>
                                  number of slices&#58; 19<br>
                                  number of bins&#58; 64,658<br>
                                  number of genes&#58; 14,270<br>
                                  number of models&#58; 11 </p>
                              </div>
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
                         <h3>L3 larva</h3>
                      </el-col>
                      <el-col :span="12">
                        <h3><a href="/vt3d_example/L3_b/index.html?atlas=/vt3d_example/L3_b" target="_blank"> Browse </a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; L3 larva of <i>drosophila</i><br>
                                  number of slices&#58; 13<br>
                                  number of bins&#58; 43,310<br>
                                  number of genes&#58; 16,326<br>
                                  number of models&#58; 13 </p>
                              </div>
                            </el-collapse-item>
                        </el-collapse  >
                      </el-col>
                   </el-row>
                  </div>
                </el-col>
                <!-- card end-->
            </el-row>

            <!-- 2023Mar addtion begin -->
            <el-row>
                <div class=upper_border>
                    <el-row>
                      <el-col :span="24"> 
                        <h2>Other Datasets</h2>
                      </el-col>
                    </el-row>
                    <!-- card begin-->
                    <el-col :span="8">
                      <div class='card'>
                       <el-row>
                          <el-col :span="24">
                            <div @click="jumpStar" >
                                <img src="./assets/STARmap.png" class="image" >
                            </div>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="12">
                             <h3>StarMap</h3>
                          </el-col>
                          <el-col :span="12">
                            <h3><a href="/vt3d_example/STARmap_3D/index.html?atlas=/vt3d_example/STARmap_3D" target="_blank"> Browse</a></h3>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="24">
                            <el-collapse>
                                <el-collapse-item   title="Summary" name="2">
                                  <div class='tutorial'>
                                      <p>
                                      sample&#58; 14h-16h embryo of <i>drosophila</i><br> <!-- TODO: -->
                                      number of slices&#58; 13<br>
                                      number of bins&#58; 15,295<br>
                                      number of genes&#58; 13,668<br>
                                      number of models&#58; 11 </p>
                                  </div>
                                </el-collapse-item>
                            </el-collapse>
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
                            <div @click="jumpSlideSeq" >
                              <img src="./assets/slide-seq.png" class="image"> 
                            </div>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="12">
                             <h3>Slide-Seq</h3>
                          </el-col>
                          <el-col :span="12">
                            <h3><a href="" target="_blank"> Browse </a></h3> <!-- TODO: -->
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="24">
                            <el-collapse>
                                <el-collapse-item   title="Summary" name="2">
                                  <div class='tutorial'> <!-- TODO: -->
                                      <p>
                                      sample&#58; 16h-18h embryo of <i>drosophila</i><br>
                                      number of slices&#58; 11<br>
                                      number of bins&#58; 14,634<br>
                                      number of genes&#58; 12,850<br>
                                      number of models&#58; 11 </p>
                                  </div>
                                </el-collapse-item>
                            </el-collapse>
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
                            <div @click="jumpFlysta" >
                              <img src="./assets/FLY.png" class="image">
                            </div>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="12">
                             <h3>Flysta3D</h3>
                          </el-col>
                          <el-col :span="12">
                            <h3><a href="/vt3d_example/E16-18h_grids_t1/index.html?atlas=/vt3d_example/E16-18h_grids_t1" target="_blank"> Browse  </a></h3>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="24">
                            <el-collapse>
                                <el-collapse-item   title="Summary" name="2">
                                  <div class='tutorial'> <!-- TODO: -->
                                      <p>
                                      sample&#58; L1 larva of <i>drosophila</i><br>
                                      number of slices&#58; 20<br>
                                      number of bins&#58; 17,787<br>
                                      number of genes&#58; 13,803<br>
                                      number of models&#58; 10 </p>
                                  </div>
                                </el-collapse-item>
                            </el-collapse  >
                          </el-col>
                       </el-row>
                      </div>
                    </el-col>
                    <!-- card end-->
                  </div>
                </el-row>
                <!-- 2023Mar addtion end --> 
              </el-col>
            

              <el-col :span="6">
                <div class=left_border>
                <el-row>
                    <!-- card begin-->
                    <el-col :span="24">
                       <el-row>
                          <el-col :span="24"> 
                            <h2>Developing Human Heart</h2>
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
                            <h3><a href="/vt3d_example/HumanHeart01/index.html?atlas=/vt3d_example/HumanHeart01" target="_blank"> Browse </a></h3>
                          </el-col>
                       </el-row>
                       <el-row>
                          <el-col :span="24">
                            <el-collapse>
                                <el-collapse-item   title="Summary" name="2">
                                  <div class='tutorial'>
                                      <p>
                                      sample&#58; developing human heart<br>
                                      number of slices&#58; 9<br>
                                      number of bins&#58; 1,467<br>
                                      number of genes&#58; 20,658<br>
                                      number of models&#58; 10 </p>
                                  </div>
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
                <el-col :span="24">
                   <el-row>
                      <el-col :span="24"> 
                        <h2>Preoptic Hypothalamic</h2>
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
                        <h3><a href="/vt3d_example/hypo_preoptic/index.html?atlas=/vt3d_example/hypo_preoptic" target="_blank"> Browse </a></h3>
                      </el-col>
                   </el-row>
                   <el-row>
                      <el-col :span="24">
                        <el-collapse>
                            <el-collapse-item   title="Summary" name="2">
                              <div class='tutorial'>
                                  <p>
                                  sample&#58; preoptic hypothalamic of mouse brain<br>
                                  number of slices&#58; 12<br>
                                  number of bins&#58; 73,655<br>
                                  number of genes&#58; 161<br>
                                  number of models&#58; 4 </p>
                              </div>
                            </el-collapse-item>
                        </el-collapse  >
                      </el-col>
                   </el-row>
                  </div>
                </el-col>
                <!-- card end-->
            </el-row>
            </div>
          </el-col>
        </el-row>
       </el-tab-pane>
       <el-tab-pane label="Tutorials" name='tutorial'>
        <h2>Tutorials to reproduce those atlases&#58;</h2>
        <el-collapse v-model="tid" accordion>
            <el-collapse-item   title="Developing drosophila embryos and larvae: E14-16h" name="1">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir E14_E16h<br>
                  cd E14_E16h<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E14-16h_a_count_normal_stereoseq.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E14-16h_a.tar.gz<br>
                  tar -xzf E14-16h_a.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E14-16h.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i E14-16h_a_count_normal_stereoseq.h5ad -o E14h_E16h_Atlas -c E14-16h.atlas.json<br>
                  cd E14h_E16h_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Developing drosophila embryos and larvae: E16-18h" name="2">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir E16_E18h<br>
                  cd E16_E18h<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E16-18h_a_count_normal_stereoseq.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E16-18h_a.tar.gz<br>
                  tar -xzf E16-18h_a.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;E16-18h.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i E16-18h_a_count_normal_stereoseq.h5ad -o E16-E18h_Atlas -c E16-E18h.atlas.json<br>
                  cd E16-18h_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Developing drosophila embryos and larvae: L1" name="3">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir L1<br>
                  cd L1<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L1_a_count_normal_stereoseq.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L1_a.tar.gz<br>
                  tar -xzf L1_a.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L1_a.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i L1_a_count_normal_stereoseq.h5ad -o L1_Atlas -c L1_a.atlas.json<br>
                  cd L1_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Developing drosophila embryos and larvae: L2" name="4">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir L2<br>
                  cd L2<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L2_a_count_normal_stereoseq.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L2_a.tar.gz<br>
                  tar -xzf L2_a.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L2_a.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i L2_a_count_normal_stereoseq.h5ad -o L2_Atlas -c L2_a.atlas.json<br>
                  cd L2_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Developing drosophila embryos and larvae: L3" name="5">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir L3<br>
                  cd L3<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L3_b_count_normal_stereoseq.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L3_b.tar.gz<br>
                  tar -xzf L3_b.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;L3_b.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;flysta3d&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i L3_b_count_normal_stereoseq.h5ad -o L3_Atlas -c L3_b.atlas.json<br>
                  cd L3_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Developing human heart" name="6">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir Heart<br>
                  cd Heart<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;heart&#47;heart3d.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;heart&#47;mesh.tar.gz<br>
                  tar -xzf mesh.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;heart&#47;heart.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;heart&#47;fixed.json<br>
                  vt3d AtlasBrowser BuildAtlas -i heart3d.h5ad -o Heart_Atlas -c heart.atlas.json<br>
                  cd Heart_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
            <el-collapse-item   title="Hypo Preoptic hypothalamic" name="7">
              <div class='tutorial'>
                  <p>
                  To reproduce this atlas&#58;<br>
                  <br>
                  1. in your terminal&#58;<br>
                  mkdir hypo_preoptic<br>
                  cd hypo_preoptic<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;merfish&#47;hypo_preoptic.h5ad<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;merfish&#47;mesh.tar.gz<br>
                  tar -xzf mesh.tar.gz<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;merfish&#47;hypo_preoptic.atlas.json<br>
                  wget -c http&#58;&#47;&#47;www.bgiocean.com&#47;vt3d_example&#47;download&#47;merfish&#47;hypo_preoptic.coord.json<br>
                  vt3d AtlasBrowser BuildAtlas -i hhypo_preoptic.h5ad -o HP_Atlas -c hypo_preoptic.atlas.json<br>
                  cd HP_Atlas &#38;&#38; vt3d AtlasBrowser LaunchAtlas -p 80<br>
                  <br>
                  2. in your web browser&#58;<br>
                  http&#58;&#47;&#47;127.0.0.1&#47;index.html
                  </p>
              </div>
            </el-collapse-item>
        </el-collapse  >
       </el-tab-pane>
       <el-tab-pane label="Resources" name='data'>
         <h3>Dataset description and data download&#58;</h3>
         <el-row>
           <el-col :span="2"><h4>name</h4></el-col>
           <el-col :span="2"><h4>spatial tech.</h4></el-col>
           <el-col :span="6"><h4>.h5ad data</h4></el-col>
           <el-col :span="3"><h4>.obj data</h4></el-col>
           <el-col :span="3"><h4>conf data</h4></el-col>
           <el-col :span="8"><h4>reference</h4></el-col>
         </el-row>
         <el-row>
           <el-col :span="2"><h5>Developing <i>drosophila</i> embryos and larvae atlas</h5></el-col>
           <el-col :span="2"><h5>Stereo-seq</h5></el-col>
           <el-col :span="12">
             <el-row>
               <el-col :span="12">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E14-16h_a_count_normal_stereoseq.h5ad" target="_blank">E14-16h_a_count_normal_stereoseq.h5ad</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E14-16h_a.tar.gz" target="_blank">E14-16h_a.tar.gz</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E14-16h.atlas.json" target="_blank">E14-16h.atlas.json</a></h5>
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/fixed.json" target="_blank">fixed.json</a></h5>
               </el-col>
             </el-row>
             <el-row>
               <el-col :span="12">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E16-18h_a_count_normal_stereoseq.h5ad" target="_blank">E16-18h_a_count_normal_stereoseq.h5ad</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E16-18h_a.tar.gz" target="_blank">E16-18h_a.tar.gz</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/E16-18h.atlas.json" target="_blank">E16-18h.atlas.json</a></h5>
               </el-col>
             </el-row>
             <el-row>
               <el-col :span="12">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L1_a_count_normal_stereoseq.h5ad" target="_blank">L1_a_count_normal_stereoseq.h5ad</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L1_a.tar.gz" target="_blank">L1_a.tar.gz</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L1_a.atlas.json" target="_blank">L1_a.atlas.json</a></h5>
               </el-col>
             </el-row>
             <el-row>
               <el-col :span="12">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L2_a_count_normal_stereoseq.h5ad" target="_blank">L2_a_count_normal_stereoseq.h5ad</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L2_a.tar.gz" target="_blank">L2_a.tar.gz</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L2_a.atlas.json" target="_blank">L2_a.atlas.json</a></h5>
               </el-col>
             </el-row>
             <el-row>
               <el-col :span="12">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L3_b_count_normal_stereoseq.h5ad" target="_blank">L3_b_count_normal_stereoseq.h5ad</a></h5>
               </el-col>
               <el-col :span="6">
                 <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L3_b.tar.gz" target="_blank">L3_b.tar.gz</a></h5>
               </el-col>
               <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/flysta3d/L3_b.atlas.json" target="_blank">L3_b.atlas.json</a></h5>
               </el-col>
             </el-row>
           </el-col>
           <el-col :span="8">
             <h5><a href="https://doi.org/10.1016/j.devcel.2022.04.006" target="_blank">Wang et al., Developmental Cell, 2022 High-resolution 3D spatiotemporal transcriptomic maps of developing Drosophila embryos and larvae </a></h5>
           </el-col>
         </el-row>

         <el-row>
           <el-col :span="2"><h5>Developing human heart atlas</h5></el-col>
           <el-col :span="2"><h5>ST</h5></el-col>
           <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/heart/heart3d.h5ad" target="_blank">heart3d.h5ad</a></h5>
           </el-col>
           <el-col :span="3">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/heart/mesh.tar.gz" target="_blank">mesh.tar.gz</a></h5>
           </el-col>
           <el-col :span="3">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/heart/heart.atlas.json" target="_blank">heart.atlas.json</a></h5>
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/heart/fixed.json" target="_blank">fixed.json</a></h5>
           </el-col>
           <el-col :span="8">
             <h5><a href="https://doi.org/10.1016/j.cell.2019.11.025" target="_blank">Asp, et al., Cell, 2019 A Spatiotemporal Organ-Wide Gene Expression and Cell Atlas of the Developing Human Heart</a></h5>
           </el-col>
         </el-row>
         <el-row>
           <el-col :span="2"><h5>Preoptic hypothalamic atlas</h5></el-col>
           <el-col :span="2"><h5>MERFISH</h5></el-col>
           <el-col :span="6">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/merfish/hypo_preoptic.h5ad" target="_blank">hypo_preoptic.h5ad</a></h5>
           </el-col>
           <el-col :span="3">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/merfish/mesh.tar.gz" target="_blank">mesh.tar.gz</a></h5>
           </el-col>
           <el-col :span="3">
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/merfish/hypo_preoptic.atlas.json" target="_blank">hypo_preoptic.atlas.json</a></h5>
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/merfish/hypo_preoptic.coord.json" target="_blank">hypo_preoptic.coord.json</a></h5>
                  <h5><a href="http://www.bgiocean.com/vt3d_example/download/merfish/hypo_preoptic.organ.json" target="_blank">hypo_preoptic.organ.json</a></h5>
           </el-col>
           <el-col :span="8">
             <h5><a href="http://dx.doi.org/10.1126/science.aau5324" target="_blank">Moffitt, et al., Science, 2018 Molecular, spatial, and functional single-cell profiling of the hypothalamic preoptic region </a></h5>
           </el-col>
         </el-row>
         <br>
         <h3>Source codes&#58;</h3>
         <el-row>
           <el-col :span="8">
             <a href="https://github.com/BGI-Qingdao/VT3D" target="_blank">Source codes of VT3D in GitHub</a><br>
           </el-col>
           <el-col :span="8">
             <a href="https://github.com/BGI-Qingdao/VT3D_Browser" target="_blank">Source codes of vt3d_browser in GitHub</a><br>
           </el-col>
           <el-col :span="8">
             <a href="https://github.com/cchd0001/VT3D_Index" target="_blank">Source codes of this homepage in GitHub</a>
           </el-col>
         </el-row>
      </el-tab-pane>
    </el-tabs>
    <hr>
    <div class='footer'>
      <el-row>
        <el-col :span="3">
            <img src="./assets/bgi.png" class="logo" >
        </el-col>
        <el-col :span="3">
            <img src="./assets/bgi_research.png" class="logo" >
        </el-col>
        <el-col :span="3">
            <img src="./assets/stomics.png" class="logo" >
        </el-col>
        <el-col :span="3">
            <img src="./assets/stomicsdb.png" class="logo" >
        </el-col>
        <el-col :span="3">
            <img src="./assets/cngb.png" class="logo" >
        </el-col>
        <el-col :span="9">
          <p>For any inquiries about the website, please contact: guolidong@genomics.cn; liyao1@genomics.cn</p>
          <p>Powered by Element.js and Echarts.js</p>
        </el-col>
      </el-row>
      <el-row>
        <el-col :span="24">
          <p>Copyright &#169; All Rights Reserved 2022 BGI Research <a href=https://beian.miit.gov.cn/>鲁ICP备2022034375号</a></p>
        </el-col>
      </el-row>
    </div>
</div>
</div>
</template>

<script>
export default {
    data() {
        return {
          tid: '1',
          activeName: 'atlas',
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
      jumpStar(){
         window.open('/vt3d_example/STARmap_3D/index.html?atlas=/vt3d_example/STARmap_3D','_blank');
      },
      jumpSlideSeq(){
         console.log('Slide-Seq data is comming soon...');
      },
      jumpFlysta(){
          window.open('/vt3d_example/E16-18h_grids_t1/index.html?atlas=/vt3d_example/E16-18h_grids_t1','_blank');
      },
    }
};
</script>

<style>
  #header-col1 {
    background-color: #4381e6;
    text-align: center;
    line-height: 100px;
    font-weight: bold;
    color: white;
  }
  .logo{
    width: 100%;
    display: block;
    margin:10px;
    padding:20px;
  }
  .footer{
    border-color: #eeeeee;
    border-style: solid;
    border-width: 1px;
    color: #8b8c8f;
    font-size: 14px;
    padding:10px;
  }
  .image {
    width: 100%;
    display: block;
  }
  .card{
     border-width: 2px;
     border-style: solid;
     border-color:#111111;
     margin:10px
  }
  .tutorial{
     background-color: #ccc;
     border-width: 2px;
     border-style: dashed;
     border-color:#111111;
     text-align: left;
     margin:10px;
     padding:10px;
  }
  .left_border{
     border-left: 3px dashed gray;
  }
  .upper_border{
     border-top: 3px dashed gray;
  }
  .center-div
  {
    margin: 0 auto;
    width: 1300px;
    background-color: white;
    padding:5px;
  }
  .background
  {
      background-color: #ccc;
  }
</style>
