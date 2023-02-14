<template>
    <section class="comments">
        <div class="container">
            <form @submit.prevent="onSubmit">
                <!-- <input v-model="comment.text" type="text" placeholder="Type your comment"> -->
                <AppTextArea v-model="comment.text"></AppTextArea>
                <!-- <button class="btn btnPrimary">Leave a comment</button> -->
                <AppButton>Leave a comment</AppButton>
            </form>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                comment: {
                    user: '',
                    text: ''
                }
            }
        },
        methods: {
            onSubmit() {
                console.log(this.comment)
                this.comment.text = ''
            }
        }
    }
</script>

<style lang="scss">
.comments {
    padding: 16px;
}

</style>