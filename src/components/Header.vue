<script>
export default{
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
    <section>
        <img :src="this.logo">
        <nav>
            <a v-for="link in links" href="link.address"> {{ link.label }}</a>     
        </nav>
    </section>
    
</template>

<style scoped>
section{
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 10vh;
    background-color: aliceblue;
}
img{
    width: 60px;
    height: 60px;
}
</style>
