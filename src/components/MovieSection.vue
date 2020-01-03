<template>
    <div class="column">
        <li class="movie-choice">
            <img :src="`${movieChoice.smallImgSrc}`" class="desktop"/>
            <p class="mobile">{{ movieChoice.subtitle }}</p>
        </li>
    </div>
</template>

<script>
    export default {
        name: "Movie",
        props : {
            movieChoice : Object
        }
    }
</script>
