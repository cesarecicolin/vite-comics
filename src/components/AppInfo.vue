<script>
export default{
    data(){
        return{
            infoPoint: [
                {
                    name: "DIGITAL COMICS",
                    img: "buy-comics-digital-comics.png"
                },
                {
                    name: "DC MERCHANDAISE",
                    img: "buy-comics-merchandise.png"
                },
                {
                    name: "SUBSCRIPTION",
                    img: "buy-comics-subscriptions.png"
                },
                {
                    name: "COMIC SHOP LOCATOR",
                    img: "buy-comics-shop-locator.png"
                },
                {
                    name: "DC POWER VISA",
                    img: "buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<template>
<section>
    <nav class="container">
        <ul>
            <li v-for="info in infoPoint">
                <img :src="`../assets/img/${info.img}`" alt="">
                <a href="">{{info.name}}</a>
            </li>
        </ul>
    </nav>
</section>
</template>

<style lang="scss" scoped>
@use "../style/partials/mixin" as *;
section{
    background-color:#0282f9;
    ul{
        @include flex(row, space-between);
            list-style: none;
            gap: 2rem;
            padding: 3rem ;
            a{
                text-decoration: none;
                color: white;
            }
    }

}
</style>