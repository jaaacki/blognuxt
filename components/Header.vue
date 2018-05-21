<template>
   <v-toolbar>
    <v-toolbar-side-icon></v-toolbar-side-icon>
    <v-toolbar-title>Title</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat @click="goToHome">Home</v-btn> 
      <v-btn flat @click="goToUser">Users</v-btn> 
      
    </v-toolbar-items>
  </v-toolbar>
</template>
<script>
export default {
    data() {
        return
        pages: [
            {name: 'Home', path: '/'},
            {name: 'Users', path: '/users'}
        ]
    },
    methods: {
        goToUser() {
            this.$router.push('/users') 
        },
        goToHome() {
            this.$router.push('/')
        }
    }
}
</script>
