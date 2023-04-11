<template>
    <HelloWorld/>
   <div class="bgdaftar">
    <div class="divpusat">
        <div class="divkiri" >
            <ComponentDaftar/>
        </div>
        <div class="divkanan">
<form class="formdaftar" action="">
    <p class="textdaftar">Username</p>
    <input placeholder="Masukkan Username" class="inpdaftar" type="text"> 
    <p class="textdaftar">Gmail</p>
    <input placeholder="Masukkan Gmail" class="inpdaftar" type="text">
    <p class="textdaftar">Password</p>
    <input placeholder="Masukkan Password" class="inpdaftar" type="password">
    <p class="textdaftar">Konfirmasi</p>
    <input placeholder="Konfirmasi Password" class="inpdaftar" type="password">
    <div class="cekbok"><input type="checkbox"><p>I Agree</p></div>
    <button class="buttondaftar" @click="$router.push('/login')">Daftar</button>
</form>
        </div>

  </div>
</div>
  </template>

<script>
import HelloWorld from '../components/HelloWorld.vue'
import ComponentDaftar from '../components/ComponentDaftar.vue'
  
export default {
  name: 'DaftarView',
  components: {
    HelloWorld, 
    ComponentDaftar
  }
}
</script>

<style>
.bgdaftar{
    background-color:#E5E5E5;
    width: 100%;
    height: 700px;
}
.divpusat{
    position: relative;
    left: 385px;
    top: 100px;
}
.divkiri{
    position: absolute;
    left: 0;
}
.divkanan{
    background-color: white;
    border-radius: 17px;
    position: absolute;
    width: 380px;
    height: 480px;
    left: 335px;

}
.textdaftar{
    margin-top: 15px;
}
.cekbok{
    display: flex;
    margin-top: 15px;
}
.formdaftar{
    margin-top: 65px;
    text-align: left;
    margin-left: 30px;
}
.inpdaftar{
    width: 300px;
    height: 30px;
    border-radius: 5px;
}
.buttondaftar{
    width: 300px;
    height: 35px;
    color: white;
    background-color: #0D6EFD;
    border: none;
    border-radius: 17px;
    font-size: 20px;
    margin-left: 5px;
    margin-top: 15px;
}
</style>