<script>
export default{
   
    nome :"Jumbotron",
    data(){
        return{
           jumbo:"img/jumbotron.jpg"
        }
    }
}
</script>

<template>
    <div id="jumbo">
        <img :src="this.jumbo">
    </div>
</template>

<style>

  img{
    width: 100%;
    height: 30%;
    object-fit: cover;
  }
</style>