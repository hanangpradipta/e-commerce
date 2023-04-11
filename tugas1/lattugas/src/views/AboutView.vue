<template>
  <HelloWorld/>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>
<script>
import HelloWorld from '../components/HelloWorld.vue'

export default {
  name: 'AboutView',
  components: {
    HelloWorld
  }
}</script>
<style>
  h1{
    margin-top: 600px;
  }
</style>
