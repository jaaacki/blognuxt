<template>
<div>
    <h1>The users view</h1>
    <nuxt-link to="/">Home</nuxt-link>

<input type="text" v-model="UserId">
<button @click="onLoadUser">Load User</button>
</div>
</template>

<script>
export default {
    data() {
        return
        UserId: ''
    },
    methods: {
        onLoadUser() {
           this.$router.push('/users/' + this.UserId)
        }
    }

}
</script>
