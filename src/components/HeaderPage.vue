<template>
    <nav class="nav">
        <a href="#">Home</a>
        <a href="#">Add Restaurant</a>
        <a href="#">Update Restaurant</a>
        <a v-on:click="logout" href="#">Log out</a>
    </nav>
</template>

<script>
    export default {
        name: 'HeaderPage',
        methods: {
            logout(){
                localStorage.clear();
                this.$router.push({name: 'LoginPage'})
            }
        }
    }
</script>



<style>
    .nav {
        background-color: #333;
        overflow: hidden;
    }

    .nav a {
        float: left;
        color: #f2f2f2;
        padding: 16px 14px;
        text-align: center;
        text-decoration: none;
        font-size: 17px;
        margin-right: 5px;
    }

    .nav a:hover {
        background-color: #ddd;
        color: #333;
    }
</style>