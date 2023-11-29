<script>
import Navbar from './Navbar.vue';
export default{
    components:{
    Navbar,
},
    nome :"Header",
    data(){
        return{
            links : [
                {
                    label: "CHARACTERS",
                    address: "#"
                },
                {
                    label: "COMICS",
                    address: "#"
                },
                {
                    label: "MOVIES",
                    address: "#"
                },
                {
                    label: "TV",
                    address: "#"
                },
                {
                    label: "GAMES",
                    address: "#"
                },
                {
                    label: "COLLECTIBLES",
                    address: "#"
                },
                {
                    label: "VIDEOS",
                    address: "#"
                },
                {
                    label: "FANS",
                    address: "#"
                },
                {
                    label: "NEWS",
                    address: "#"
                },
                {
                    label: "SHOP",
                    address: "#"
                },

            ],
            logo : "/img/dc-logo.png" 

        }
    }
}

</script>

<template>
    <header>
        <div id="header-cont">
            <section>
               <img :src="this.logo">
               <div class="navbar-cont">
                  <Navbar v-for="link in links" href="link.address" :menulinks="link"/>
               </div>          
            </section>
        </div>   
    </header>    
</template>

<style scoped>
header{
    background-color: aliceblue;
}
#header-cont{
    width: 80vw;
    margin-right: auto;
    margin-left: auto;
}
.navbar-cont{
    display: flex;
}
section{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 10vh;
}
img{
    width: 60px;
    height: 60px;
}

</style>
