<template>
    <section class="menu">
        <div class="menu-wrapper">
            <nuxt-link to="/">Home</nuxt-link>
            <nuxt-link to="/admin/new-post">New post</nuxt-link>
            <p>Exit</p>
        </div>
    </section>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss">
.menu-wrapper {
    display: flex;
    align-items: flex-end;
    flex-wrap: nowrap;
    flex-direction: column;
    padding: 16px;
    text-align: end;
    min-width: 110px;
}

</style>