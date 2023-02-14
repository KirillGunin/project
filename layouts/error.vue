<template>
    <section class="not-found">
        <div class="container">
            <div class="not-found__wrapper">
                <p class="title">Page not found</p>
                <nuxt-link to="/">Home page</nuxt-link>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss">
.not-found__wrapper {
    // margin: auto;
    // text-align: center;
    display: flex;
    margin-top: 100px;
    flex-direction: column;
    align-items: center;
}
</style>