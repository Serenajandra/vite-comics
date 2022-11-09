<script>
export default{
    name: "AppTeamTitansBanner",

    data(){
        return{
            title:"TitansBanner",
            imgName:"banner"
        }
    },
    methods: {
        getImage(image){
            return new URL(image, import.meta.url).href
        }
    }
}
</script>

<template>
    <div class="banner-container">
        <img :src="getImage(`../assets/img/jumbotron.jpg`)" alt="{`title`}">
    </div>
</template>

<style lang="scss" scoped>
.banner-container{
    background-color: aquamarine;
    width: 100%;
    height: 300px;
}
</style>