<script>
    export default{
       name: "AppBlueNav",
        data(){
            return {
                blueLinks: [
                    {
                        title: "digital comics",
                        image: `buy-comics-digital-comics.png`,
                        href: "/digital comics",
                        active: false
                    },
                    {
                        title: "dc merchandise",
                        image: `buy-comics-merchandise.png`,
                        href: "/dc merchandise",
                        active: false
                    },
                    {
                        title: "subscription",
                        image: `buy-comics-subscriptions.png`,
                        href: "/subscription",
                        active: false
                    },
                    {
                        title: "comic shop locator",
                        image: `buy-comics-shop-locator.png`,
                        href: "/comic shop locator",
                        active: false
                    },
                    {
                        title: "dc power visa",
                        image: `buy-dc-power-visa.svg`,
                        href: "/dc power visa",
                        active: false
                    }
                ]
            }
        },
        methods: {
            getImagePath(imgPath){
                return new URL (imgPath, import.meta.url).href
            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <nav>
                <ul>
                    <li v-for="(blueLink, index) in blueLinks" :key="index" >
                        <img :src="getImagePath(`../assets/img/${blueLink.image}`)">
                        <a :href="blueLink.href" :class="{active : blueLink.active}">{{blueLink.title.toUpperCase()}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variabiles" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/general.scss" as *;
    .container{
        width: 100%;
        min-height: 150px;
        background-color: lighten($primary-color, 15%);
        @include flex-center ("both");
        
    }

    ul{
        @include flex-center ("horizontal");
        

        li{
            font-size: 0.7rem;
            @include flex-center ("both");
            
            img{
                width: 40px;
                margin-right: 1rem;
            }
            
            a{
                color: white;
            }
        }
    }
</style>