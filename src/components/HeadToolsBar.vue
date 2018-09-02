<template>
  <v-toolbar color="amber" app absolute clipped-left>
    <v-toolbar-side-icon @click.native="drawer = !drawer"></v-toolbar-side-icon>
    <span class="title ml-3 mr-5">Échange&nbsp;<span class="font-weight-light">Cli</span></span>
    <v-text-field
      solo-inverted
      flat
      hide-details
      label="Search"
      prepend-inner-icon="search"
    ></v-text-field>
    <v-spacer></v-spacer>
  </v-toolbar>
</template>

<script>
    export default {
        name: "HeadToolsBar"
    }
</script>

<style scoped>

</style>
