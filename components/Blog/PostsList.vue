<template>
    <section class="posts-list">
        <!-- <div class="container"> -->
            <div class="posts__wrapper">
                <PostPreview
                    v-for="post in posts"
                    :key="post.id"
                    :admin="admin"
                    :post="post"
                />
            </div>
        <!-- </div> -->
    </section>
</template>

<script>
import PostPreview from '@/components/Blog/PostPreview.vue'
    export default {
        components: { PostPreview},
        props: {
            posts: {
                type: Array,
                required: true
            },
            admin: {
                type: Boolean,
                default: false
            }
        }
    }
</script>

<style lang="scss">
    .posts__wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
    }
</style>