<script>
    
    export default{
        name: "AppFooter",
        data (){
            return{
                comicsLinks: [

                ]
            }
        }
    }
</script>
<template>
<footer>
    <div class="footer-top">
        <div class="row">
            <div class="col">
                <h3>DC Comics</h3>
                <ul>   
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                    <li>link</li>
                </ul>
                <h3>Shop</h3>
                <ul>
                    <li>link</li>
                    <li>link</li>
                </ul>
            </div>
        
            <div class="col">
                <h3>DC</h3>
                <ul>
                    <li>link</li>
                    <li>link</li>
                </ul>
            </div>
            <div class="col">
                <h3>Sites</h3>
                <ul>
                    <li>link</li>
                    <li>link</li>
                </ul>
            </div>
        </div>
        <div class="dc-logo">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    
    <div class="footer-bottom">
        <div class="btn-container">
            <button class="btn-border-blue">sign-up-now!</button>
        </div>
        <div class="social-links">
            <ul>
                <li><button class="btn-social">follow us</button></li>
                <li> <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a> </li>
                <li> <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a> </li>
                <li> <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a> </li>
                <li> <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a> </li>
                <li> <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a> </li> 
            </ul>
        </div>
    </div>

</footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;
@use "../styles/general.scss" as *;
@use "../styles/partials/variabiles" as *;

.footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    width: 100%;
    height: 400px;
    display: flex;
    .row{
        width: 40%;
        margin-left: 10rem;
        padding-top: 2rem;
        margin-bottom: 2rem;
        display: flex;
        justify-content: space-between;
        border: 1px solid green;

        h3{
            color: white;
            padding-top: 0.8rem;
            text-transform: uppercase;
        }

        li{
            line-height: 2rem;
            color: grey;
            margin: 0;
            padding-top: 0.5rem;
        }
    }  
    .dc-logo{
        width: 50%;
        height: 100%;
        margin-left: 10rem;
        img{
            object-fit: cover;
            width: 100%;
            height: 100%;
            
    
        }
   }
}

.footer-bottom{
    width: 100%;
    height: 80px;
    background-color: rgb(48, 48, 48);
    display: flex;
    align-items: center;
    justify-content: space-around;

    .btn-border-blue{
        width: 10rem;
        border: 1px solid lighten($primary-color, 15%);
        background-color:transparent;
        padding: .8rem 1rem;
        color:white;
        text-transform: uppercase;
    }
    .social-links{
        width: 30%;
        padding: .8rem 1rem;
        ul{
            display: flex;
            align-items: center;
        }

        .btn-social{
            color: lighten($primary-color, 25%);
            background-color: transparent;
            text-transform: uppercase;
            border: none;
        }

    }
}

</style>
