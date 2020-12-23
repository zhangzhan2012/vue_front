<template>
  <div class="content">
    <div>
      <el-row :gutter="0">
        <el-carousel :interval="3000" arrow="never" height="620px" >
          <el-carousel-item v-for="item in dataimg" :key="item">
            <div class="grid-content">
              <el-col :md="12" :offset="6">
                <div>
                  <img :src="item.src">
                </div>
              </el-col>
            </div>
          </el-carousel-item>
        </el-carousel>
      </el-row>
    </div>
    <div>
      <el-row>
        <el-col :span="4" style="text-align: center">
          ¥396.00起
        </el-col>
        <el-col :span="20">
        </el-col>
      </el-row>
    </div>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      dataimg: [{
        src: require('../../static/img/1.gif')
      },
      {
        src: require('../../static/img/2.jpg')
      }
      ]
    }
  }

}
</script>

<style scoped>
.content{
  width: 800px !important;
  text-align: center;
}
</style>
