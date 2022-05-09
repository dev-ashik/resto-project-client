<template>
    <h1>This is Home page</h1>
</template>

<script>
export default {
    name: 'HomePage',
    mounted() {
        let user = localStorage.getItem('user-info');
        if (!user) {
            this.$router.push({ name: 'SignUp' })
        }
    }
}
</script>