<template>
  <div>
      <h1>Users</h1>      
      <input type="text" v-model="userId"></input>
      <button @click="onLoadUser">Load User</button>
  </div>
</template>

<script>
export default {
    data() {
        return{
            userId:''
        }
    },
    methods: {
        onLoadUser() {
            this.$router.push('/users/' + this.userId)

        }
    }
}
</script>
