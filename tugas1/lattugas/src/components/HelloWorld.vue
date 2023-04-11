<template>
  <div class="head">
    <div class="atur">
    <nav><tr>
   <td> <router-link class="route" to="/">Home</router-link>| </td>
   <td> <router-link class="route" to="/about">Discount</router-link>| </td>
    <td> <router-link class="route" to="/about">Category</router-link> </td>
  </tr>
  </nav>
 <h2>Shop</h2>
 <form action="">
 <input type="text" placeholder="Search product...">
 <button class="search"><img class="img1" src="../assets/Vector.png" alt=""></button> </form>
 <button class="keranjang"><img class="img2" src="../assets/keranjang.png" alt=""></button> 
 <button class="login" @click="$router.push('/login')">Login</button> 

  </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.head{
  background-color: #0D6EFD;
  width: 100%;
  height: 100px;
}
.atur{
  position: absolute;
  left: 50px;
  top: 5px;
}

nav{
  position: absolute;
  left: 40px;
  top: -23px;
  color: white;
}
.route{
  color: white;
  text-decoration: none;
  margin-left: 35px;
  font-size: 23px;
  font-family: sans-serif;
}
h2{
  position: absolute;
  left: 110px;
  top: 35px;
  color: white;
  font-size: 38px;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
input{
  position: absolute;
  width: 700px;
  left: 350px;
  top: 50px;
  height: 30px;
  border-radius: 8px;
  border: none;
}
.keranjang{
  position: absolute;
    top: 49px;
    left: 1070px;
    width: 80px;
    height: 33px;
    border: solid 2px white;
    background-color: transparent;
    border-radius: 8px;
}
.img2{
  width: 20px;
  margin-top: 3px;
}
.search{
  position: absolute;
  top: 51px;
  left: 1003px;
  border-radius: 8px;
  width: 50px;
  height: 30px;
  border: none;
  background-color: #0D6EFD;
}
.img1{
  width: 20px;
  margin-top: 3px;
}
.login{
  position: absolute;
    top: 49px;
    left: 1170px;
    width: 80px;
    height: 33px;
    border: solid 2px white;
    background-color: transparent;
    border-radius: 8px;
    color: white;
}
a{
  font-weight: 200;
  font-size: 14px !important;
}
</style>
