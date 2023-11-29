<script>
export default{
    nome :"FooterTop",
    data(){
        return{
           footerBg: "/img/footer-bg.jpg",
           footer2Bg:"/img/dc-logo-bg.png",
           current:0,
           infos: [
            {
                titolo: "DC COMICS",
                info: [
                    "1",
                    "2"
                ]
            }, 
            {
                titolo: "DC",
                info: [
                    {
                        desc:"1",
                    },
                    {
                        desc:"2",
                    },
                    {
                        desc:"3",
                    }
                ]
            },
            {
                titolo: "SHOP",
                info: [
                    {
                        desc:"1",
                    },
                    {
                        desc:"2",
                    },
                    {
                        desc:"3",
                    }
                ]
            },         
           ]
        }
    }
}
</script>

<template>
    <div id="footerBG">
        <img :src="this.footerBg" id="bg-foot1">
        <div class="square">
            <img :src="this.footer2Bg" class="bg-foot2">
        </div>
        <div class="footer-mini-contain">
            <ul  v-for= "( informazione , current) in infos">{{ informazione.titolo }}
                <li>{{ informazione.info[current]}}</li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
*{
    color: aliceblue;
}
#bg-foot1{ 
    width: 100%;
    height: 50vh;
    object-fit: cover;
}
.square{
    width: 500px;
    height: 50vh;
    transform: translate(160% , -100%);
}
.square > img {
    width: 100%;
    height: 100%;
    object-fit: cover;

}
#footerBG{
    height: 50vh;
}
.footer-mini-contain{
    background-color: rgba(95, 158, 160, 0.395);
    width: 20%;
    transform: translate(80% , -400%);
}
</style>