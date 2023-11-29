<script>
import FooterICN from './FooterICN.vue'

export default{
    components:{
       FooterICN
    },
    nome :"Footer",
    data(){
        return{
           
        }
    }
}
</script>

<template>
    <div id="bg-footer">
        <div id="footer-container">
            <div class="lft-foot">
                <button>SING-UP NOW</button>
            </div>
            <div class="rgt-foot">
                <FooterICN />
            </div>
        </div>
    </div>
    

</template>

<style scoped>
#footer-container{
    display: flex;
    justify-content: space-between;
    width: 80vw;
}
#bg-footer{
    background-color: rgba(43, 49, 45, 0.32);
    height: 10vh;
    display: flex;
    justify-content: center;
}
</style>