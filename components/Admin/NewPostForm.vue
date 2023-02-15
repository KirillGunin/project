<template>
    <section class="new-post">
        <h1 class="title">New post</h1>
        <form class="new-post__form" @submit.prevent>
            <AppInput v-model="post.title" />
            <AppInput v-model="post.img"/>
            <AppTextArea v-model="post.description"/>
            <div class="controls">
                <AppButton @click="onSubmit">Add post</AppButton>
                <AppButton class="btnDanger" @click.prevent="cancel">Cancel</AppButton>
            </div>
        </form>
    </section>
</template>

<script>
    export default {
        props: {
            postEdit: {
                type: Object,
                required: false
            }
        },
        data() {
            return {
                post: this.postEdit
                ?
                {...this.postEdit}
                :
                {
                    id: '',
                    title: '',
                    img: '',
                    description: '',
                }
            }
        },
        methods: {
            onSubmit() {
                this.$emit('submit', this.post)
            },
            cancel() {
                this.$router.push('/admin/')
            }
        }
    };
</script>

<style lang="scss">
.new-post {
    max-width: 600px;
    margin: 0 auto;
    text-align: center;
    &__form{
        margin: 16px;
    }
}
</style>
