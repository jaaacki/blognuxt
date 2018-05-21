<template>
  <v-app>
    <Header></Header>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
   
  </v-app>
</template>

<script>
  import Header from '~/components/Header'

  export default {
    data() {
      return {
      }
    },
    components: {
    Header
  }
}
</script>
