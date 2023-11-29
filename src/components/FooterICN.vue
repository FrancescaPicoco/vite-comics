<script>
export default{
    nome:"FooterICN",
    props:["footerIcnProps"],
    data(){
        return{            
        }
    }
}
</script>

<template>
    <div id="footerICNcont">
        <div  class="footerICNcont">
            <span>{{ footerIcnProps.follow }}</span>
            <img :src="footerIcnProps.socialIcn">
        </div>
    </div>    
</template>

<style scoped>
#footerICNcont{
  display: flex;
  align-items: center;
}
.footerICNcont{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0.5rem;
}
span{
    color: rgb(49, 49, 206);
}
</style>