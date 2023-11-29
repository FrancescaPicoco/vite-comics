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

<style scoped>
#jumbo{
    height: 50vh;
}
  img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
</style>