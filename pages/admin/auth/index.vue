<template>
    <div class="wrapper-content wrapper-content--fixed">
        <div class="container">
            <section class="auth">
                <h1 class="title">Login</h1>
                <form @submit.prevent="onSubmit" class="auth__form">
                    <AppInput v-model="user.mail" placeholder="login"/>
                    <AppInput v-model="user.password" placeholder="password"/>
                    <div class="controls">
                        <p class="controls-item">Registrate</p>
                        <AppButton class="controls-item">Login</AppButton>
                    </div>
                </form>
            </section>
        </div>
    </div>
</template>

<script>
export default {
data() {
    return {
        user: {
            mail: '',
            password: ''
        }
    }
},
methods: {
    onSubmit() {
        console.log(this.user)
        this.user = {}
    }
}
    
}
</script>

<style lang="scss">
.auth {
    max-width: 600px;
    margin: 0 auto;
    text-align: center;
    border: solid 1px #aaaad555;
    border-radius: 10px;
    box-shadow: 0px 0px 10px 5px rgba(194,194,194,0.5);
    -webkit-box-shadow: 0px 0px 10px 5px rgba(194,194,194,0.5);
    -moz-box-shadow: 0px 0px 10px 5px rgba(194,194,194,0.5);
    &__form{
        margin: 16px;
    }
}
.controls {
    display: flex;
    justify-content: center;
    align-items: center;
    &-item {
        margin: 0 20px;
        cursor: pointer;
    }
}
</style>