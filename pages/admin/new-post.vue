<template>
    <div class="wrapper-content wrapper-content--fixed">
        <div class="container">
            <NewPostForm @submit="onSubmit"/>
        </div>
    </div>
</template>

<script>
    import NewPostForm from '@/components/Admin/NewPostForm.vue'
    export default {
        components: { NewPostForm },
        layout: 'admin',
        methods: {
            onSubmit(post) {
                console.log(post)
                
            }
        }
    }
</script>

<style lang="scss">

</style>