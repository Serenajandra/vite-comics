<script>
import { stringifyStyle } from '@vue/shared';

export default{
    name: "AppComicCard",

    props: {
        thumb: String, 
        price: String,
        series: String,
        type: String
    }
}
</script>

<template>

    <div class="col card">
        <img :src="thumb" :alt="series">
        <p>{{series}}</p>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;
    .card{
        width: calc(100% / 6 - 0.5rem - 1rem);
        margin: 0 0.5rem;  

        img{
            object-fit: cover;
            width: 100%;
            height: 50%;
        }

        p{
            color: white;
        }
    }

</style>