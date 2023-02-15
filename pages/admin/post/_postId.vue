<template>
    <div class="wrapper-content wrapper-content--fixed">
        <div class="container">
            <NewPostForm @submit="onSubmit" :postEdit="post"/>
        </div>
    </div>
</template>

<script>
    import NewPostForm from '@/components/Admin/NewPostForm.vue'
    export default {
        components: { NewPostForm },
        layout: 'admin',
        data() {
            return {
                post: {id: 1, title: 'lalka', description: 'bla bla', img: 'https://www.blessthisstuff.com/imagens/stuff/the-heritage-chief.jpg'},
            }
        },
        methods: {
            onSubmit(post) {
                console.log(post)
                
            }
        }
    }
</script>

<style lang="scss">

</style>