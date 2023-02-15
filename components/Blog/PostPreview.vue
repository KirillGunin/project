<template>
    <nuxt-link :to="getLink" class="post-preview">
        <img :src="post.img" :alt="post.title">
        <div class="post-content">
            <h3 class="title">{{ post.title }}</h3>
            <p class="description">{{ post.description }}</p>
        </div>
    </nuxt-link>
</template>

<script>
    export default {
        props: {
            post: {
                type: Object,
                required: true
            },
            admin: {
                type: Boolean,
                default: false
            }
        },
        computed: {
            getLink() {
                return this.admin ? `/admin/post/${this.post.id}` : `/blog/post/${this.post.id}`
            }
        }
    }
</script>

<style lang="scss">
.post-preview {
    max-width: 33%;
    padding: 16px;
    // margin-bottom: 20px;
    text-align: start;
    height: auto;
    img {
        margin-bottom: 16px;
    }
}
</style>