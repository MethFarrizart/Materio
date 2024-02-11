<template>
  <v-app>
    <v-main>
      <materio/>
    </v-main>
  </v-app>
</template>

<script>
import materio from './components/materio.vue'

export default {
  name: 'App',

  components: {
    materio,
  },

  data: () => ({
    //
  }),
}
</script>
