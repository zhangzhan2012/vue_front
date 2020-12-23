<template>
  <div>
    <iframe src="/page.html" frameborder="0" name="showHere" scrolling=auto width='1000px' height='400px'></iframe>
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
</style>
