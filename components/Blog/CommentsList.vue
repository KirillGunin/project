<template>
    <section class="comments-list" v-if="comments">
        <div class="container" v-for="(comment, index) in comments" :key="index">
            <div class="comment">
                <p>{{ comment.user }}</p>
                <p>{{ comment.text }}</p>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
     props: {
        comments: {
            type: Array,
            default: null
        }
     }   
    }
</script>

<style lang="scss">
.comments-list{
    padding: 16px;
}
.comment {
    padding: 5px;
    padding-left: 10px;
}
</style>