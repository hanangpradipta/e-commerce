<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <ImgboxHome/>
    <DiskonHome/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import ImgboxHome from '@/components/ImgboxHome.vue'
import DiskonHome from '@/components/DiskonHome.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    ImgboxHome,
    DiskonHome
  }
}
</script>
 <style>
*{
  margin: 0;
}
.imgboxhome{
  margin-top: 20px;
}
</style>