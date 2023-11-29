<script>
export default{
    nome :"Services",
    data(){
        return{ 
            icons:[
                {
                    icn:"/img/buy-comics-digital-comics.png",
                    decription:"DIGITAL COMICS"
                },
                {
                    icn:"/img/buy-comics-merchandise.png",
                    decription:"DC MERCHANDISE"
                },
                {
                    icn:"/img/buy-comics-subscriptions.png",
                    decription:"SUBSCRIPTIONS"
                },
                {
                    icn:"/img/buy-comics-shop-locator.png",
                    decription:"COMIC SHOP LOCATOR"
                },
                {
                    icn:"/img/buy-dc-power-visa.svg",
                    decription:"DC POWER VISA"
                },
            ]
        }      
    }
}
</script>

<template>
    <div id="blueone">
        <div id="container-serv">
            <div id="icn-card" v-for="card in icons">
                <div id="single-card">
                    <img :src="card.icn">
                    <span>{{card.decription}}</span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
#blueone{
    background-color: rgb(2, 130, 249);
}
#container-serv{
    width: 80vw;
    height: 15vh;
    margin-right: auto;
    margin-left: auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
}
#single-card{
    display: flex;
    align-items: center;
    margin: 0 1rem;
}
img{
    width: 35px;
}
span{
    font-size: 16px;
}
</style>
