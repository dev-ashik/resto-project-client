<template>
    <HeaderPage/>
    <h1>This is Home page</h1>
</template>

<script>
import HeaderPage from "./HeaderPage.vue";
export default {
    name: "HomePage",
    mounted() {
        let user = localStorage.getItem("user-info");
        if (!user) {
            this.$router.push({ name: "SignUp" });
        }
    },
    components: { HeaderPage }
}
</script>