<template>
    <div class="intro">
        <h1>{{ title }}</h1>
        <p>elkremlkm rlekmlekrf erfrfr rf rf er f erg tg htrhrthtrgerf wed wef erg t htrhhtrfefwd</p>
        <p>elkremlkm rlekmlekrf erfrfr rf rf er f erg tg htrhrtrfefwd</p>
        <p>elkremlkm rlekmlekrf erfrfr rfg htrhrthtrgerf wed wef erg t htrhhtrfefwd</p>
        <p>elkremlkm rlekmlekrhhtrfefwd</p>

    </div>
</template>

<script>
    export default {
        props: {
            title: {
                type: String,
                required: true
            }
        }
    }
</script>

<style lang="scss">
    .intro {
        margin: 0;
        text-align: start;
        background: white;
        opacity: 70%;
        padding: 16px;
        border-radius: 10px;
    }
</style>