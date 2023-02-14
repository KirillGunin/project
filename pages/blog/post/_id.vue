<template>
    <div class="wrapper-content wrapper-content--fixed">
        <Post :post="post"/>
        <CommentForm />
        <CommentsList :comments="comments"/>
  </div>
</template>

<script>
import Post from '@/components/Blog/Post.vue'
import CommentForm from '@/components/Blog/CommentForm.vue'
import CommentsList from '@/components/Blog/CommentsList.vue'

    export default {
        components: {Post, CommentForm, CommentsList },
        data() {
            return {
                post: {
                    id: 1, title: 'lalka', description: 'bla bla', img: 'https://www.blessthisstuff.com/imagens/stuff/the-heritage-chief.jpg',
                },
                comments: [
                    {
                        user: 1,
                        text: 'qwe'
                    },
                    {
                        user: 2,
                        text: 'qwffrfe'
                    },
                    {
                        user: 3,
                        text: 'qwssssssssssse'
                    },
                ]

            }
        }
    }
</script>

<style lang="scss">
.post {
    // display: flex;
    // flex-direction: column;
    // align-items: center;
    // justify-content: center;
    // padding: 0 16px;
}
.post-header {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    padding: 0 16px;
    margin-bottom: 20px;
    
}
.image {
    width: 600px;
    margin-bottom: 20px;
}
.kkk {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 0 16px;
}


</style>