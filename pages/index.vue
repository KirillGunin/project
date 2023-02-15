<template>
    <div class="wrapper-content wrapper-content--fixed">
      <div class="container">
        <PostsList :posts="posts"/>
      </div>
    </div>
</template>

<script>
import PostsList from '@/components/Blog/PostsList.vue'
export default {
  components: { PostsList },
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
