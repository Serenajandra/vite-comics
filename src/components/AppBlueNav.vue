<script>
    export default{
       name: "AppBlueNav",
       date(){
        return {
            links: [
                {
                    title: "digital comics",
                    image: "C:\Boolean corso\vite-comics\src\assets\img\buy-comics-digital-comics.png",
                    href: "/digital comics",
                    active: "false"
                },
                {
                    title: "dc merchandise",
                    image: "",
                    href: "/dc merchandise",
                    active: "false"
                },
                {
                    title: "subscription",
                    image: "",
                    href: "/subscription",
                    active: "false"
                },
                {
                    title: "comic shop locator",
                    image: "",
                    href: "/comic shop locator",
                    active: "false"
                },
                {
                    title: "dc power visa",
                    image: "",
                    href: "/dc power visa",
                    active: "false"
                }
            ]
        }
       }
    }
</script>

<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(link, index) in links" :key="index">>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <a href="">link</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variabiles" as *;
    .container{
        width: 100%;
        min-height: 200px;
        background-color: lighten($primary-color, 15%);
    }
</style>