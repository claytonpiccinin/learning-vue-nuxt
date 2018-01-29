<template>
    <v-toolbar color="cyan lighten-2">
      <v-form @submit="submit">
          <v-text-field
            solo
            label="Pesquisar"
            append-icon="search"
            prepend-icon="search"
          ></v-text-field>
        </v-form>
    </v-toolbar>
</template>

<script>
  export default {
    components : {
    },
    data (){
      return {
        search : ''
      }
    },
    methods: {
      submit(event){
        this.$router.push('resultados')
      }
    }
  }
</script>