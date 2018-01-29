<template>
    <v-toolbar color="cyan">
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
    data () {
      return {
        search: 'tst'
      }
    },
    methods: {
      submit(event){
        this.$router.push('resultados')
      }
    }
  }
</script>