<script>
export default {
    data() {
        return{
            link: [
                {
                    title: "CHARACTRES"
                },
                {
                    title: "COMICS"
                },
                {
                    title: "MOVIES"
                },
                {
                    title: "TV"
                },
                {
                    title: "GAMES"
                },
                {
                    title: "COLLECTIBLES"
                },
                {
                    title: "VIDEOS"
                },
                {
                    title: "FANS"
                },
                {
                    title: "NEWS"
                },
                {
                    title: "SHOP"
                }
            ]
        }
    }
}
</script>

<template>
<header>
    <div class="header-contain container" >
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
          <ul>
            <li v-for="link in link" key="link.title">
                <a href="">{{ link.title }}</a>
            </li>
          </ul>
        </nav>
        
    </div>
</header>
</template>

<style lang="scss" scoped>
@use "../style/partials/mixin" as *;
header{
    padding: 2rem;
    .header-contain{
        @include flex(row, space-between);
        ul{
            @include flex(row, space-between);
            list-style: none;
            gap: 2rem;
            a{
                text-decoration: none;
                color: black;
                
                &:hover{
                    color: #0282f9;
                }
            }
                    
                
        
        }
        
    }
}
</style>