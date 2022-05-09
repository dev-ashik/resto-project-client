<template>
    <img class="logo" src="../assets/resto-logo.png" alt="">
    <h1>Sign Up</h1>
    <div class="login">
        <input type="text" v-model="email" placeholder="Enter Email">
        <input type="password" v-model="password" placeholder="Enter Password">
        <button v-on:click="login">Login</button>
        <p>
            <router-link to="/sign-up">Sign Up</router-link>
        </p>
    </div>
</template>

<script>
export default {
    name: 'LoginPage',
    data() {
        return {
            email: '',
            password: ''
        }
    },
    methods: {
        login(){
            console.log(this.email, this.password);
        }   
    }


}
</script>



<style>

</style>