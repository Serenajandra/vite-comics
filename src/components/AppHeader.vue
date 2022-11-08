<script>
export default{
   name: "AppHeader"
}
</script>

<template>
    <header>
        <div class="logo"><a href=""><img src="../assets/img/dc-logo.png" alt="dcLogo"></a></div>
        <nav>
            <ul>
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
                <li><a href="">link</a></li> 
            </ul>
        </nav>
    </header>

    </template>

<style lang="scss" scoped>
 @use "../styles/partials/mixins.scss" as *;
 @use "../styles/general.scss" as *;

header{
    display: flex;
    align-items: center;
    width: 100%;
    height: 80px;
    background-color: aquamarine;
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
}



</style>