<script>
export default{
   name: "AppHeader",
   data(){
    return{
        links: [
            {
                title: "characters",
                href:"/characters",
                active: false,
            },
            {
                title: "comics",
                href: "/comics",
                active: false,
            },
            {
                title: "movies",
                href: "/movies",
                active: false,
            },
            {
                title: "tv",
                href: "/tv",
                active: false,
            },
            {
                title: "games",
                href: "/games",
                active: false,
            },
            {
                title: "collectibles",
                href: "/collectibles",
                active: false,
            },
            {
                title: "videos",
                href: "/videos",
                active: false,
            },
            {
                title: "fans",
                href: "/fans",
                active: false,
            },
            {
                title: "news",
                href: "/news",
                active: false,
            },
            {
                title: "shop",
                href: "/shop",
                active: false,

            }
        ]
    }
   }
}
</script>

<template>
    <header>
        <div class="logo"><a href=""><img src="../assets/img/dc-logo.png" alt="dcLogo"></a></div>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :class="{ active : link.active}" :href="link.href">{{link.title.toUpperCase()}}</a>
                </li> 
            </ul>
        </nav>
    </header>

</template>

<style lang="scss" scoped>
 @use "../styles/partials/mixins.scss" as *;
 @use "../styles/general.scss" as *;
 @use "../styles/partials/variabiles" as *;

header{
    display: flex;
    align-items: center;
    width: 100%;
    height: 80px;
    .logo{
        width: 40%;
        height: 100%;
        text-align: center;

        img{
            width: 60px;
            margin-top: 10px;
            vertical-align: middle;
        }
    }
}

ul{
    @include flex-center ("horizontal");

    li{
        font-size: 0.7rem;
    }

    a:hover,
    .active {
        color: $primary-color;
        border-bottom: 5px solid $primary-color;
        padding-bottom: 30px;
    }
}
</style>