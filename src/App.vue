<template>
  <v-app>
    <div id=app>
      <DesertList v-bind:is-visible="showCommand"></DesertList>

      <v-switch
        v-model="showCommand"
        color="red darken-4"
        label="Toggle Show"
      ></v-switch>
    </div>
  </v-app>
</template>

<script>
import DesertList from './components/DesertList'

export default {
  name: 'App',
  components: {
    DesertList
  },
  data () {
    return {
      showCommand: true,
    }
  }
}
</script>
