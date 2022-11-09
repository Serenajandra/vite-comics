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

    <div class="card">
        <img :src="thumb" :alt="series">
        <p>{{series.toUpperCase()}}</p>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;
    .card{
        width: calc(100% / 6 - 0.5rem - 1rem);
        margin: 0 0.5rem;  
        padding: 1.5rem 0;

        img{
            object-fit: cover;
            width: 100%;
            height: 12rem;
        }

        p{
            color: white;
            font-size: 0.6rem;
            padding-top: 0.3rem;
        }
    }

</style>