<script>
export default{
    nome :"FooterTop",
    data(){
        return{
           footerBg: "/img/footer-bg.jpg",
           infos: [
            {
                titolo: "DC COMICS",
                info: [
                    "prova uno" ,
                    "prova due" ,
                    "prova tre"
                ]
            },
           
           
           ]
        }
    }
}
</script>

<template>
    <div id="footerBG">
        <img :src="this.footerBg">
        <div class="footer-mini-contain">
            <ul  v-for= "( informazione ) in infos">{{ informazione.titolo }}
                <li>{{this.info}}</li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
*{
    color: aliceblue;
}
img{ 
    width: 100%;
    height: 50vh;
    object-fit: cover;
}
#footerBG{
    height: 50vh;
}
.footer-mini-contain{
    background-color: rgba(95, 158, 160, 0.395);
    width: 20%;
    transform: translate(80% , -850%);
}

</style>