<template>
    <HelloWorld/>
    <div class="bg">
    <div class="log">
      <form class="form1" action="">
        <input class="user" type="text" placeholder="Username"> <br>
        <input class="pass" type="password" placeholder="Password"> <br>
        <button class="log2" @click="$router.push('/')">Login</button> 
      </form>
    </div>
        <p class="buat">Belum punya akun? <router-link to="/daftar">Daftar</router-link></p>
  </div>
  </template>
  <script>
  // @ is an alias to /src
  import HelloWorld from '../components/HelloWorld.vue'
  
  export default {
    name: 'LoginView',
    components: {
      HelloWorld
    }
  }
  </script>
  <style>
.log{
  position: absolute;
    background-color: white;
    height: 405px;
    width: 542px;
    margin-top: 125px;
    margin-left: 445px;
    border-radius: 17px;
}
.bg{
  margin-top: 0;
  background-color:#E5E5E5 ;
  height: 710px;
}
.form1{
  margin-top: 100px;
}
.user{
  width: 450px;
  height: 50px;
  text-align: center;
  font-size: 30px;
  border: none;
  border-bottom: solid;
  border-color: rgb(144, 144, 144);

}
.pass{
  width: 450px;
  height: 50px;
  text-align: center;
  font-size: 30px;
  border: none;
}
.log2{
  margin-top: 30px;
  width: 450px;
  height: 50px;
  background-color: #0D6EFD;
  border-radius: 8px;
  border: none;
  color: white;
  font-size: 25px;;
}
.buat{
  position: absolute;
  top: 645px;
  left: 590px;
  font-size: 20px;
}

</style>
