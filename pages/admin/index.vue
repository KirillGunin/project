<template>
    <div class="wrapper-content wrapper-content--fixed">
        <div class="container">
            <!-- <h1 class="title">Admin page</h1> -->
            <div class="admin-content">
                <PostsList :posts="posts"/>
                <Menu />
            </div>
        </div>
    </div>
</template>
  
<script>
import PostsList from '~/components/Blog/PostsList.vue'
import Menu from '~/components/UI/Menu.vue'
export default {
layout: 'admin',
components: { PostsList, Menu },
    data() {
        return {
            posts: [
                {id: 1, title: 'lalka', description: 'bla bla', img: 'https://www.blessthisstuff.com/imagens/stuff/the-heritage-chief.jpg'},
                {id: 2, title: 'lol', description: 'bla bla', img: 'https://www.fixie75.com/wp-content/uploads/2018/05/fixie75-state_bicycle_co_rutherford_3_blue_fixie_12-1.jpg'},
                {id: 3, title: 'kek', description: 'bla bla', img: 'https://i.pinimg.com/originals/c0/1f/c2/c01fc2c00f539c5a2d5e50a827e36ce6.jpg'}
            ]
        }
    }
}
</script>

<style lang="scss">
.admin-content {
    display: flex;
}
</style>