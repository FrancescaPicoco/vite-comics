<script>
export default{
    props:["details"]
}
</script>

<template>   
    <div class="card">
    <img :src="details.thumb">
    <span>{{ details.series }}</span>      
    </div>  
</template>

<style scoped>
   .card{
    width: calc((100% / 6) - 2rem);
    height: 200px;
    margin: 1rem;
   }
   img{
    width: 100%;
    height: 100%;
   }
</style>