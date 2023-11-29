<script>
export default{
    nome:"FooterICN",
    data(){
        return{            
            icons:[
                {
                    follow: "FOLLOW US",
                },
                {
                    socialIcn : 'img/footer-facebook.png'
                },
                {
                    socialIcn : 'img/footer-twitter.png'
                },
                {
                    socialIcn : 'img/footer-youtube.png'
                },
                {
                    socialIcn : 'img/footer-pinterest.png'
                },
                {
                    socialIcn : 'img/footer-periscope.png'
                },
            ]
        }
    }
}
</script>

<template>
    <div id="footerICNcont">
        <div v-for="iconafooter in icons" class="footerICNcont">
            <span>{{ iconafooter.follow }}</span>
            <img :src="iconafooter.socialIcn">
        </div>
    </div>    
</template>

<style scoped>
#footerICNcont{
    display: flex;
    justify-content: center;
    align-items: center;
}
.footerICNcont{
    display: flex;
    align-items: center;
    justify-content: center;
}
span{
    color: rgb(49, 49, 206);
}
</style>