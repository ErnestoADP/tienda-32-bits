<template>
  <div class="py-5 text-start">
    <h1>Página no existente</h1>
    <img src="../assets/img/404.gif" alt="">
    <div id="buttom">
    <router-link  class="btn btn-dark btn-lg" to="/">Volver a Inicio</router-link>
    </div>

    
  </div>
</template>

<script>
export default {
  name: "NotFound",
};
</script>
<style>
img{
  width: 100%;
  height: 700px;
 
}

#buttom,h1{
  margin: 0.5rem;
  text-align: center;
 
}
</style>
