<template>
    <div class="wrapper-content wrapper-content--fixed">
        <!-- <section class="post">
            <div class="container">
                <div class="post-header">
                    <img class="image" :src="post.img" :alt="post.title">
                    <h1 class="title">{{ post.title }}</h1>
                </div>
                <div class="kkk">
                    123
                </div>
            </div>
        </section> -->
        <Post :post="post"/>
  </div>
</template>

<script>
import Post from '@/components/Blog/Post.vue'
    export default {
        components: {Post },
        data() {
            return {
                post: {
                    id: 1, title: 'lalka', description: 'bla bla', img: 'https://www.blessthisstuff.com/imagens/stuff/the-heritage-chief.jpg',
                }
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