<template>
    <section class="post">
        <div class="container">
            <div class="post-header">
                <img class="image" :src="post.img" :alt="post.title">
                <h1 class="title">{{ post.title }}</h1>
            </div>
            <div class="kkk">
                123
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        props: {
            post: {
                type: Object,
                required: true
            }
        }
    }
</script>

<style lang="scss">

</style>