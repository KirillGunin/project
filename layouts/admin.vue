<template>
    <div class="wrapper">
        <Header />
        <Nuxt />
    </div>
</template>

<script>
import Header from '@/components/system/Header.vue'
    export default {
        components: { Header },
        middleware: ['auth']
    }
</script>

<style lang="scss">

</style>